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
DELETE /v2/chapters/96
Content-Type: application/json
Authorization: Bearer fe45d39ca75ff23814a92ffbba9e70b0fc3101d8f49a25d0ac8eba17e50e4526
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/96" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe45d39ca75ff23814a92ffbba9e70b0fc3101d8f49a25d0ac8eba17e50e4526"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/98
Content-Type: application/json
Authorization: Bearer e0f1845fcd68fd1756e9756d8110956411e854c401e0b1d9f91d10748df7d0a9
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
    "id": 98,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-20T19:31:49.685Z",
    "course_id": 117,
    "author_id": 423,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-20T19:31:49.171Z",
    "questions_updated_at": "2016-10-20T19:31:49.171Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 426,
        "chapter_id": 98,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:49.632Z",
        "created_at": "2016-10-20T19:31:49.632Z",
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
        "author_id": 427,
        "chapter_id": 98,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:49.669Z",
        "created_at": "2016-10-20T19:31:49.669Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 424,
        "chapter_id": 98,
        "position": 48,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:49.378Z",
        "created_at": "2016-10-20T19:31:49.274Z",
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
            "id": 106,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 107,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 425,
        "chapter_id": 98,
        "position": 49,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:49.563Z",
        "created_at": "2016-10-20T19:31:49.449Z",
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
            "id": 108,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 109,
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
curl "api.goskive.com/v2/chapters/98" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0f1845fcd68fd1756e9756d8110956411e854c401e0b1d9f91d10748df7d0a9"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/91
Content-Type: application/json
Authorization: Bearer 0e062cbfd14b953753e088d914d4f62803195f3aa2fee48c4362055fc1224c86
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
    "id": 91,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-20T19:31:47.950Z",
    "course_id": 110,
    "author_id": 403,
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
curl "api.goskive.com/v2/chapters/91" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e062cbfd14b953753e088d914d4f62803195f3aa2fee48c4362055fc1224c86"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/23
Content-Type: application/json
Authorization: Bearer 2bef51badd594cf6515dd710a04017355a746c77cec4b82fc3aec323aec33f09
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bef51badd594cf6515dd710a04017355a746c77cec4b82fc3aec323aec33f09"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 7dfbf33d3eff4452ab1b35651f11d7237700cb0751683c54a9b6d74193a8fe20
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
      "id": 25,
      "author_id": 891,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:32.726Z",
      "status": "published",
      "subject_id": 274,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 893,
      "reply_to_id": 25,
      "created_at": "2016-10-20T19:32:32.807Z",
      "status": "published",
      "subject_id": 275,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 895,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:32.891Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 897,
      "reply_to_id": 27,
      "created_at": "2016-10-20T19:32:32.974Z",
      "status": "published",
      "subject_id": 277,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 899,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:33.054Z",
      "status": "reported",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 901,
      "reply_to_id": 29,
      "created_at": "2016-10-20T19:32:33.134Z",
      "status": "published",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 903,
      "reply_to_id": 29,
      "created_at": "2016-10-20T19:32:33.216Z",
      "status": "published",
      "subject_id": 280,
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
	-H "Authorization: Bearer 7dfbf33d3eff4452ab1b35651f11d7237700cb0751683c54a9b6d74193a8fe20"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d2bee1d7f1bce5fe243fff5b70870baca3e5ec73888c8f55d69d388ba19839cd
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
      "author_id": 921,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:33.971Z",
      "status": "published",
      "subject_id": 288,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 923,
      "reply_to_id": 39,
      "created_at": "2016-10-20T19:32:34.055Z",
      "status": "published",
      "subject_id": 289,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 925,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:34.137Z",
      "status": "published",
      "subject_id": 290,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 927,
      "reply_to_id": 41,
      "created_at": "2016-10-20T19:32:34.247Z",
      "status": "published",
      "subject_id": 291,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 929,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:34.338Z",
      "status": "reported",
      "subject_id": 292,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 931,
      "reply_to_id": 43,
      "created_at": "2016-10-20T19:32:34.423Z",
      "status": "published",
      "subject_id": 293,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 933,
      "reply_to_id": 43,
      "created_at": "2016-10-20T19:32:34.511Z",
      "status": "published",
      "subject_id": 294,
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
	-H "Authorization: Bearer d2bee1d7f1bce5fe243fff5b70870baca3e5ec73888c8f55d69d388ba19839cd"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 2c295ca7ef74aed293f6d45468fb6a71ebdd0abb2c03e3cae5b4c0055424d86d
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
      "id": 47,
      "author_id": 938,
      "reply_to_id": 46,
      "created_at": "2016-10-20T19:32:34.745Z",
      "status": "published",
      "subject_id": 296,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 942,
      "reply_to_id": 48,
      "created_at": "2016-10-20T19:32:34.919Z",
      "status": "published",
      "subject_id": 298,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 946,
      "reply_to_id": 50,
      "created_at": "2016-10-20T19:32:35.094Z",
      "status": "published",
      "subject_id": 300,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 948,
      "reply_to_id": 50,
      "created_at": "2016-10-20T19:32:35.184Z",
      "status": "published",
      "subject_id": 301,
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
	-H "Authorization: Bearer 2c295ca7ef74aed293f6d45468fb6a71ebdd0abb2c03e3cae5b4c0055424d86d"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer aab383b752cb458264c2cd1d4eba0b1e01f333dab8de12850bfff2b3af684234
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
      "id": 57,
      "author_id": 959,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:32:35.686Z",
      "status": "reported",
      "subject_id": 306,
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
	-H "Authorization: Bearer aab383b752cb458264c2cd1d4eba0b1e01f333dab8de12850bfff2b3af684234"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer 15424ffaba16f707d922ff8b0a96f808a6366f517fd79d782ad69d6d20f51454
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15424ffaba16f707d922ff8b0a96f808a6366f517fd79d782ad69d6d20f51454"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/205/chapters
Content-Type: application/json
Authorization: Bearer 04d4c219fbfc5028a471d5fb6ba80f3b43f6d63e6a8814d0eba9a4e3aad76d7f
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
    "id": 146,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T19:32:07.649Z",
    "course_id": 205,
    "author_id": 664,
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
curl "api.goskive.com/v2/courses/205/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04d4c219fbfc5028a471d5fb6ba80f3b43f6d63e6a8814d0eba9a4e3aad76d7f"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0a7b7b347342e2a4490a4479b03b04729537a592b02b04e88ec9f7bdc5ad491a
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
    "id": 147,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T19:32:07.783Z",
    "course_id": 206,
    "author_id": 666,
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
	-H "Authorization: Bearer 0a7b7b347342e2a4490a4479b03b04729537a592b02b04e88ec9f7bdc5ad491a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ae31c4b884b3de53c02faf046c8fb5ea00aa1bee2e830eb41f594e74f5e48f49
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
      "id": 134,
      "title": "Clever Chapter Title 113",
      "position": 1,
      "updated_at": "2016-10-20T19:32:06.275Z",
      "course_id": 199,
      "author_id": 639,
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
      "id": 135,
      "title": "Clever Chapter Title 114",
      "position": 2,
      "updated_at": "2016-10-20T19:32:06.299Z",
      "course_id": 199,
      "author_id": 640,
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
      "id": 136,
      "title": "Clever Chapter Title 115",
      "position": 3,
      "updated_at": "2016-10-20T19:32:06.553Z",
      "course_id": 199,
      "author_id": 641,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-20T19:32:06.203Z",
      "questions_updated_at": "2016-10-20T19:32:06.203Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae31c4b884b3de53c02faf046c8fb5ea00aa1bee2e830eb41f594e74f5e48f49"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e996df3576da883f230681902c3c37354190682cd6746f58d5f425abe9c68002
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
      "id": 137,
      "title": "Clever Chapter Title 116",
      "position": 1,
      "updated_at": "2016-10-20T19:32:06.792Z",
      "course_id": 201,
      "author_id": 648,
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
      "id": 138,
      "title": "Clever Chapter Title 117",
      "position": 2,
      "updated_at": "2016-10-20T19:32:06.817Z",
      "course_id": 201,
      "author_id": 649,
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
      "id": 139,
      "title": "Clever Chapter Title 118",
      "position": 3,
      "updated_at": "2016-10-20T19:32:06.842Z",
      "course_id": 201,
      "author_id": 650,
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
	-H "Authorization: Bearer e996df3576da883f230681902c3c37354190682cd6746f58d5f425abe9c68002"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/218
Content-Type: application/json
Authorization: Bearer da752e3f60dffa6a241e4a8c0b541ddb36e33999490b8217a1f0755786f46980
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/218" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da752e3f60dffa6a241e4a8c0b541ddb36e33999490b8217a1f0755786f46980"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3fd768a6b574eef03d73434ca75d0a8b734030b7f939513e2dd679d941b02e03
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
	-H "Authorization: Bearer 3fd768a6b574eef03d73434ca75d0a8b734030b7f939513e2dd679d941b02e03"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 7ee2073493baf9bad14be7c71b21df0455f4800481e2f1a3f7d59f1533972b30
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
    "creator_id": 693,
    "id": 211,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 195,
    "additional_university_ids": [

    ],
    "topic_id": 216,
    "discipline_id": 216,
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
    "chapters_updated_at": "2016-10-20T19:32:13.240Z",
    "updated_at": "2016-10-20T19:32:14.768Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 153,
        "title": "Clever Chapter Title 129",
        "position": 1,
        "updated_at": "2016-10-20T19:32:14.721Z",
        "course_id": 211,
        "author_id": 693,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-20T19:32:13.240Z",
        "questions_updated_at": "2016-10-20T19:32:13.240Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 154,
        "title": "Clever Chapter Title 130",
        "position": 2,
        "updated_at": "2016-10-20T19:32:14.761Z",
        "course_id": 211,
        "author_id": 693,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-20T19:32:13.240Z",
        "questions_updated_at": "2016-10-20T19:32:13.240Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 693,
        "chapter_id": 153,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.556Z",
        "created_at": "2016-10-20T19:32:14.556Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 693,
        "chapter_id": 154,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.628Z",
        "created_at": "2016-10-20T19:32:14.628Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 693,
        "chapter_id": 153,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.597Z",
        "created_at": "2016-10-20T19:32:14.597Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 693,
        "chapter_id": 154,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.670Z",
        "created_at": "2016-10-20T19:32:14.670Z",
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
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 696,
        "chapter_id": 153,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.710Z",
        "created_at": "2016-10-20T19:32:14.710Z",
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
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 697,
        "chapter_id": 154,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:14.750Z",
        "created_at": "2016-10-20T19:32:14.750Z",
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
	-H "Authorization: Bearer 7ee2073493baf9bad14be7c71b21df0455f4800481e2f1a3f7d59f1533972b30"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/216
Content-Type: application/json
Authorization: Bearer 69b8ac176a041283b3c7a7e031c12a0ca348aaa838415d105e7b649d7e87f689
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
    "creator_id": 710,
    "id": 216,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 200,
    "additional_university_ids": [

    ],
    "topic_id": 221,
    "discipline_id": 221,
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
    "updated_at": "2016-10-20T19:32:16.948Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/216" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69b8ac176a041283b3c7a7e031c12a0ca348aaa838415d105e7b649d7e87f689"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer af02c56616fe4dab4779178e1eec98039293e2bf01c2fccff5fac523ec941e5a
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
    "creator_id": 707,
    "id": 214,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 198,
    "additional_university_ids": [

    ],
    "topic_id": 219,
    "discipline_id": 219,
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
    "updated_at": "2016-10-20T19:32:16.684Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af02c56616fe4dab4779178e1eec98039293e2bf01c2fccff5fac523ec941e5a"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 05bc6e2f197e01b9dd5841f811cf05995ad104c82b9b025d4a8aaabd87996646
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
      "user_id": 140,
      "feedbackable_id": 22,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:27.644Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 144,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:27.952Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 148,
      "feedbackable_id": 24,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:28.244Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 152,
      "feedbackable_id": 25,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:28.544Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 156,
      "feedbackable_id": 26,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-20T19:31:28.844Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05bc6e2f197e01b9dd5841f811cf05995ad104c82b9b025d4a8aaabd87996646"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 97ba5cccbb81ba33e8de3c040a330ca80480b4c2852caaab1b8c1f769e6417d8
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
      "id": 19,
      "user_id": 135,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-20T19:31:27.326Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97ba5cccbb81ba33e8de3c040a330ca80480b4c2852caaab1b8c1f769e6417d8"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 1740dc76f7267b19cdf7a2966c623094b11c296a9cb659dc9ff0343fc18900be
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1740dc76f7267b19cdf7a2966c623094b11c296a9cb659dc9ff0343fc18900be"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 0aecb4151231b86b9f205439da5a5d67d29fc1f5a85e7e84794e5471987f37f3
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
    "id": 8,
    "uploader": {
      "id": 445,
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
      "created_at": "2016-10-20T19:31:50.982Z",
      "updated_at": "2016-10-20T19:31:50.982Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-20T19:31:51.059Z",
    "updated_at": "2016-10-20T19:31:51.059Z",
    "course_id": 122,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aecb4151231b86b9f205439da5a5d67d29fc1f5a85e7e84794e5471987f37f3"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/92/feedbacks
Content-Type: application/json
Authorization: Bearer f5793c23ffb63570bc177d4662c8119fb04dcd689ef4eb83204d9eb34d4eeaa9
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
      "user_id": 769,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:32:21.303Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 768,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:32:21.293Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/92/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5793c23ffb63570bc177d4662c8119fb04dcd689ef4eb83204d9eb34d4eeaa9"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5805b88fb14320ff9579b91181abdba9899aa13496a4c1c12076d28e011f317e
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
      "author_id": 255,
      "chapter_id": 52,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:36.436Z",
      "created_at": "2016-10-20T19:31:36.436Z",
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
      "author_id": 258,
      "chapter_id": 53,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:36.583Z",
      "created_at": "2016-10-20T19:31:36.583Z",
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
      "author_id": 261,
      "chapter_id": 54,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:36.720Z",
      "created_at": "2016-10-20T19:31:36.720Z",
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
      "author_id": 264,
      "chapter_id": 55,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:36.860Z",
      "created_at": "2016-10-20T19:31:36.860Z",
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
      "author_id": 267,
      "chapter_id": 56,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:36.995Z",
      "created_at": "2016-10-20T19:31:36.995Z",
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
	-H "Authorization: Bearer 5805b88fb14320ff9579b91181abdba9899aa13496a4c1c12076d28e011f317e"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 5b496c3708ac79b9c5818a664e662d5aee5cbd4a35ea7aede6a27da698dda4a8
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
      "author_id": 283,
      "chapter_id": 61,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:37.745Z",
      "created_at": "2016-10-20T19:31:37.745Z",
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
	-H "Authorization: Bearer 5b496c3708ac79b9c5818a664e662d5aee5cbd4a35ea7aede6a27da698dda4a8"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/republish
Content-Type: application/json
Authorization: Bearer 3495be4c668db4d04faf230682150eb223f495a99033d0db9b6a505dc146e669
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3495be4c668db4d04faf230682150eb223f495a99033d0db9b6a505dc146e669"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/59/feedbacks
Content-Type: application/json
Authorization: Bearer 179d4857870e5079ea9ab46ff9a0e65fd65c6c8846905271462f757736dab4fd
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
      "id": 32,
      "user_id": 484,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:53.890Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 483,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:53.878Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/59/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 179d4857870e5079ea9ab46ff9a0e65fd65c6c8846905271462f757736dab4fd"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer bd1d91a8e606e16711cc202c01a2fc73fac2fd0931c381a4b4bb4f796d614d7c
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
      "id": 125,
      "obfuscated_id": "K6zw0Yc6Me8",
      "author_id": 844,
      "chapter_id": 186,
      "position": 117,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:27.940Z",
      "created_at": "2016-10-20T19:32:27.805Z",
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
          "id": 252,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 253,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 835,
      "chapter_id": 183,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:27.014Z",
      "created_at": "2016-10-20T19:32:26.883Z",
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
          "id": 246,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 247,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 838,
      "chapter_id": 184,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:27.311Z",
      "created_at": "2016-10-20T19:32:27.178Z",
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
          "id": 248,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 249,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 841,
      "chapter_id": 185,
      "position": 116,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:27.611Z",
      "created_at": "2016-10-20T19:32:27.477Z",
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
          "id": 250,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 251,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 126,
      "obfuscated_id": "fKTMLttUR-w",
      "author_id": 847,
      "chapter_id": 187,
      "position": 118,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:28.230Z",
      "created_at": "2016-10-20T19:32:28.104Z",
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
          "id": 254,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 255,
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
	-H "Authorization: Bearer bd1d91a8e606e16711cc202c01a2fc73fac2fd0931c381a4b4bb4f796d614d7c"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9d0568799ecedeb71409beead7938b625aa4f7418e1918933a19ca2d26d78311
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
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 831,
      "chapter_id": 182,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:32:26.673Z",
      "created_at": "2016-10-20T19:32:26.545Z",
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
          "id": 244,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 245,
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
	-H "Authorization: Bearer 9d0568799ecedeb71409beead7938b625aa4f7418e1918933a19ca2d26d78311"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/128/republish
Content-Type: application/json
Authorization: Bearer 9d418cf07ca069d40e50e4d2c208bd8a7231393607f645f8969c5b8255c1fe52
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/128/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d418cf07ca069d40e50e4d2c208bd8a7231393607f645f8969c5b8255c1fe52"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8b5f7204b1d7b47b29120e633450c0148f914a8d58b463fb988d5b971e8cb89b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":184,"published":false}}
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
    "creator_id": 570,
    "id": 179,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "topic_id": 184,
    "discipline_id": 184,
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
    "updated_at": "2016-10-20T19:32:01.256Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":184,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b5f7204b1d7b47b29120e633450c0148f914a8d58b463fb988d5b971e8cb89b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2bf65cce6f51129b9b78b3d80a0d8921434a90d9dc7ca9ab9aa74c70878892da
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
      "creator_id": 559,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 175,
      "discipline_id": 175,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
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
      "updated_at": "2016-10-20T19:32:00.282Z",
      "shortname": "fu-course-148"
    },
    {
      "creator_id": 559,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
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
      "updated_at": "2016-10-20T19:32:00.321Z",
      "shortname": "fu-course-149"
    },
    {
      "creator_id": 560,
      "id": 172,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
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
      "updated_at": "2016-10-20T19:32:00.366Z",
      "shortname": "fu-course-150"
    },
    {
      "creator_id": 560,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
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
      "chapters_updated_at": "2016-10-20T19:32:00.651Z",
      "updated_at": "2016-10-20T19:32:00.658Z",
      "shortname": "fu-course-151"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bf65cce6f51129b9b78b3d80a0d8921434a90d9dc7ca9ab9aa74c70878892da"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b371a0db181ac555c5c7d9e2abb20a412c855bc96fb925d5d025fbf964e94746
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
      "creator_id": 566,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
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
      "updated_at": "2016-10-20T19:32:00.852Z",
      "shortname": "fu-course-152"
    },
    {
      "creator_id": 566,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 153",
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
      "updated_at": "2016-10-20T19:32:00.890Z",
      "shortname": "fu-course-153"
    },
    {
      "creator_id": 567,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-154",
      "html_url": "https://goskive.com/course/fu-course-154",
      "slug": "fu-course-154",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 154",
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
      "updated_at": "2016-10-20T19:32:00.936Z",
      "shortname": "fu-course-154"
    },
    {
      "creator_id": 567,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-155",
      "html_url": "https://goskive.com/course/fu-course-155",
      "slug": "fu-course-155",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
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
      "updated_at": "2016-10-20T19:32:00.974Z",
      "shortname": "fu-course-155"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b371a0db181ac555c5c7d9e2abb20a412c855bc96fb925d5d025fbf964e94746"
```
