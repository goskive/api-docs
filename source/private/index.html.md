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
DELETE /v2/chapters/54
Content-Type: application/json
Authorization: Bearer a056f3b697002e019f70580748279d2ee9ce65691f5aa7dd843a5692eeeee63b
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a056f3b697002e019f70580748279d2ee9ce65691f5aa7dd843a5692eeeee63b"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/61
Content-Type: application/json
Authorization: Bearer 0b5647f7b711924914e3de9b1458ec005729b66942bf34a48222b809a7228d70
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
    "id": 61,
    "updated_at": "2016-11-09T13:23:46.792Z",
    "course_id": 73,
    "author_id": 240,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-09T13:23:46.181Z",
    "questions_updated_at": "2016-11-09T13:23:46.181Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 243,
        "chapter_id": 61,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:46.732Z",
        "created_at": "2016-11-09T13:23:46.732Z",
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
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 244,
        "chapter_id": 61,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:46.772Z",
        "created_at": "2016-11-09T13:23:46.772Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 241,
        "chapter_id": 61,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:46.430Z",
        "created_at": "2016-11-09T13:23:46.296Z",
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
            "id": 141,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 142,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 242,
        "chapter_id": 61,
        "position": 57,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:46.653Z",
        "created_at": "2016-11-09T13:23:46.511Z",
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
            "id": 143,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 144,
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
curl "api.goskive.com/v2/chapters/61" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b5647f7b711924914e3de9b1458ec005729b66942bf34a48222b809a7228d70"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/57
Content-Type: application/json
Authorization: Bearer f7b1537110ffd3fe22aeda6c07590eb93c9b50ef42bcbc7badbf652e285d5f76
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
    "id": 57,
    "updated_at": "2016-11-09T13:23:45.078Z",
    "course_id": 69,
    "author_id": 225,
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
curl "api.goskive.com/v2/chapters/57" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7b1537110ffd3fe22aeda6c07590eb93c9b50ef42bcbc7badbf652e285d5f76"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/12
Content-Type: application/json
Authorization: Bearer ddb7671d6775a4d1bd0a4b1526dff0e0a03b0511730587dd82d7cc1cfede5d28
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddb7671d6775a4d1bd0a4b1526dff0e0a03b0511730587dd82d7cc1cfede5d28"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e082ba44ac584c8f34350e63b3f78d88b531a71b9389834f6b11f7db256c9270
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
      "id": 15,
      "author_id": 596,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:15.689Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 598,
      "reply_to_id": 15,
      "created_at": "2016-11-09T13:24:15.791Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 600,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:15.885Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 602,
      "reply_to_id": 17,
      "created_at": "2016-11-09T13:24:15.977Z",
      "status": "published",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 604,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:16.068Z",
      "status": "reported",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 606,
      "reply_to_id": 19,
      "created_at": "2016-11-09T13:24:16.156Z",
      "status": "published",
      "subject_id": 162,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 608,
      "reply_to_id": 19,
      "created_at": "2016-11-09T13:24:16.249Z",
      "status": "published",
      "subject_id": 163,
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
	-H "Authorization: Bearer e082ba44ac584c8f34350e63b3f78d88b531a71b9389834f6b11f7db256c9270"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2bb2cf90b5cf25a1c9aeb1d3689228a5d71d4c535efcc9d605c26253dbca4cef
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
      "id": 30,
      "author_id": 628,
      "reply_to_id": 29,
      "created_at": "2016-11-09T13:24:17.235Z",
      "status": "published",
      "subject_id": 172,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 630,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:17.336Z",
      "status": "published",
      "subject_id": 173,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 632,
      "reply_to_id": 31,
      "created_at": "2016-11-09T13:24:17.437Z",
      "status": "published",
      "subject_id": 174,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 634,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:17.535Z",
      "status": "reported",
      "subject_id": 175,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 636,
      "reply_to_id": 33,
      "created_at": "2016-11-09T13:24:17.666Z",
      "status": "published",
      "subject_id": 176,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 638,
      "reply_to_id": 33,
      "created_at": "2016-11-09T13:24:17.761Z",
      "status": "published",
      "subject_id": 177,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 626,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:17.127Z",
      "status": "published",
      "subject_id": 171,
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
	-H "Authorization: Bearer 2bb2cf90b5cf25a1c9aeb1d3689228a5d71d4c535efcc9d605c26253dbca4cef"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 70df8c27c268bc36707405e123893573ab6a75f611c1735b15213d82d5688039
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
      "author_id": 658,
      "reply_to_id": 43,
      "created_at": "2016-11-09T13:24:18.679Z",
      "status": "published",
      "subject_id": 186,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 662,
      "reply_to_id": 45,
      "created_at": "2016-11-09T13:24:18.857Z",
      "status": "published",
      "subject_id": 188,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 666,
      "reply_to_id": 47,
      "created_at": "2016-11-09T13:24:19.030Z",
      "status": "published",
      "subject_id": 190,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 668,
      "reply_to_id": 47,
      "created_at": "2016-11-09T13:24:19.116Z",
      "status": "published",
      "subject_id": 191,
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
	-H "Authorization: Bearer 70df8c27c268bc36707405e123893573ab6a75f611c1735b15213d82d5688039"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 0c909328c1cb52086e9c0bc2f07c8125804551423e06fc79dfdba3b2b0d7ff38
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
      "author_id": 649,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:18.286Z",
      "status": "reported",
      "subject_id": 182,
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
	-H "Authorization: Bearer 0c909328c1cb52086e9c0bc2f07c8125804551423e06fc79dfdba3b2b0d7ff38"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/9/republish
Content-Type: application/json
Authorization: Bearer 036483676861d9901e208b20d135722c9e8c3742e2fd09dc81c5f0934b44b946
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 036483676861d9901e208b20d135722c9e8c3742e2fd09dc81c5f0934b44b946"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/103/chapters
Content-Type: application/json
Authorization: Bearer 12c0871c7cebe36ad4941fffbf0e4665a26e7501a88508de8ab3d6572ada478b
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
    "id": 90,
    "updated_at": "2016-11-09T13:23:56.627Z",
    "course_id": 103,
    "author_id": 375,
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
curl "api.goskive.com/v2/courses/103/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12c0871c7cebe36ad4941fffbf0e4665a26e7501a88508de8ab3d6572ada478b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b52125e1337efbc2715fcbe130914604b0e6d0eb1a1e53431aa2c9f59e861b9d
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
    "updated_at": "2016-11-09T13:23:56.799Z",
    "course_id": 104,
    "author_id": 377,
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
	-H "Authorization: Bearer b52125e1337efbc2715fcbe130914604b0e6d0eb1a1e53431aa2c9f59e861b9d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b71cfff480f5f40c9f5b184f853bef3d2f50aa7cdfb6e79a3cbfae54cd7f8a33
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
      "id": 108,
      "updated_at": "2016-11-09T13:23:59.036Z",
      "course_id": 115,
      "author_id": 415,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 90",
      "position": 1
    },
    {
      "id": 109,
      "updated_at": "2016-11-09T13:23:59.063Z",
      "course_id": 115,
      "author_id": 416,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 91",
      "position": 2
    },
    {
      "id": 110,
      "updated_at": "2016-11-09T13:23:59.356Z",
      "course_id": 115,
      "author_id": 417,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-09T13:23:58.955Z",
      "questions_updated_at": "2016-11-09T13:23:58.955Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 92",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b71cfff480f5f40c9f5b184f853bef3d2f50aa7cdfb6e79a3cbfae54cd7f8a33"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 12b6286e3ab5422c32e409666f3139326de80882059f7ad38116715ece093c78
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
      "id": 111,
      "updated_at": "2016-11-09T13:23:59.623Z",
      "course_id": 117,
      "author_id": 424,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 93",
      "position": 1
    },
    {
      "id": 112,
      "updated_at": "2016-11-09T13:23:59.649Z",
      "course_id": 117,
      "author_id": 425,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 94",
      "position": 2
    },
    {
      "id": 113,
      "updated_at": "2016-11-09T13:23:59.678Z",
      "course_id": 117,
      "author_id": 426,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 95",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12b6286e3ab5422c32e409666f3139326de80882059f7ad38116715ece093c78"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1c501ede4bca5e38e1e357d119cb6c69f1763e3da2376322b9fefdbdf29a1975
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
	-H "Authorization: Bearer 1c501ede4bca5e38e1e357d119cb6c69f1763e3da2376322b9fefdbdf29a1975"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/60
Content-Type: application/json
Authorization: Bearer 8ad02e6419afab790708e209a4439ebb1eb8d659e31e400bf7391e69f0cca6b5
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/60" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ad02e6419afab790708e209a4439ebb1eb8d659e31e400bf7391e69f0cca6b5"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 973a5e8344e0b146126b7a172d67d0e834a71cdb7209dafcf7453fa02e6c6bd8
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
    "creator_id": 142,
    "id": 43,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 43,
    "additional_university_ids": [

    ],
    "discipline_id": 46,
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
    "chapters_updated_at": "2016-11-09T13:23:32.778Z",
    "updated_at": "2016-11-09T13:23:34.333Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 142,
        "chapter_id": 39,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.114Z",
        "created_at": "2016-11-09T13:23:34.114Z",
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
        "author_id": 142,
        "chapter_id": 40,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.189Z",
        "created_at": "2016-11-09T13:23:34.189Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 142,
        "chapter_id": 39,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.156Z",
        "created_at": "2016-11-09T13:23:34.156Z",
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
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 142,
        "chapter_id": 40,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.231Z",
        "created_at": "2016-11-09T13:23:34.231Z",
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
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 145,
        "chapter_id": 39,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.273Z",
        "created_at": "2016-11-09T13:23:34.273Z",
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
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 146,
        "chapter_id": 40,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.314Z",
        "created_at": "2016-11-09T13:23:34.314Z",
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
        "id": 39,
        "updated_at": "2016-11-09T13:23:34.285Z",
        "course_id": 43,
        "author_id": 142,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T13:23:32.778Z",
        "questions_updated_at": "2016-11-09T13:23:32.778Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 33",
        "position": 1
      },
      {
        "id": 40,
        "updated_at": "2016-11-09T13:23:34.325Z",
        "course_id": 43,
        "author_id": 142,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T13:23:32.778Z",
        "questions_updated_at": "2016-11-09T13:23:32.778Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 34",
        "position": 2
      }
    ],
    "topic_id": 46,
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
	-H "Authorization: Bearer 973a5e8344e0b146126b7a172d67d0e834a71cdb7209dafcf7453fa02e6c6bd8"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/50
Content-Type: application/json
Authorization: Bearer 6cdcc1b6039bab2966947cf92ce7640e151858b7759d1241cee63b704e89bb63
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
    "creator_id": 170,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 50,
    "additional_university_ids": [

    ],
    "discipline_id": 53,
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
    "updated_at": "2016-11-09T13:23:40.229Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 53,
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
curl "api.goskive.com/v2/courses/50" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cdcc1b6039bab2966947cf92ce7640e151858b7759d1241cee63b704e89bb63"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 156f2cf109326df66499ffab23e5004f148be66e4cc3a9c8d9e75d8a3944dbc6
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
    "creator_id": 167,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 48,
    "additional_university_ids": [

    ],
    "discipline_id": 51,
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
    "updated_at": "2016-11-09T13:23:39.770Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 51,
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
	-H "Authorization: Bearer 156f2cf109326df66499ffab23e5004f148be66e4cc3a9c8d9e75d8a3944dbc6"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer c530daf8767514deecfe6b43c14eb09e93a8f421acbdfe340a8343407b093bee
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
      "id": 15,
      "user_id": 314,
      "feedbackable_id": 80,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:23:52.069Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 318,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:23:52.389Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 322,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:23:52.718Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 326,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:23:53.155Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 330,
      "feedbackable_id": 84,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T13:23:53.490Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c530daf8767514deecfe6b43c14eb09e93a8f421acbdfe340a8343407b093bee"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer b18944506e8aa66149598f8499ec53df839987705ddc9e51fca4247b1b18b380
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
      "id": 24,
      "user_id": 351,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T13:23:55.206Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b18944506e8aa66149598f8499ec53df839987705ddc9e51fca4247b1b18b380"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 1b588b6d535e68574ac7f27b27dc7c1d18d54a4414ff7d36959aa658e77ea86c
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
	-H "Authorization: Bearer 1b588b6d535e68574ac7f27b27dc7c1d18d54a4414ff7d36959aa658e77ea86c"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer 7c76bd88203120e99c360db984c54b6cb2ceb478e74457971b2a3660b6774c9e
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
      "id": 793,
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
      "created_at": "2016-11-09T13:24:29.698Z",
      "updated_at": "2016-11-09T13:24:29.698Z"
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
    "created_at": "2016-11-09T13:24:29.772Z",
    "updated_at": "2016-11-09T13:24:29.772Z",
    "course_id": 258,
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
	-H "Authorization: Bearer 7c76bd88203120e99c360db984c54b6cb2ceb478e74457971b2a3660b6774c9e"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/54/feedbacks
Content-Type: application/json
Authorization: Bearer 74d3920b9a9619707d655b792702a2d5623cd6398762a2b16960837c6a051f97
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
      "feedbackable_id": 54,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:08.502Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 533,
      "feedbackable_id": 54,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:08.491Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/54/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74d3920b9a9619707d655b792702a2d5623cd6398762a2b16960837c6a051f97"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer c8b29ecc1979e88fbc8c29015117234aa41bd030cbe9ca4893d78d0f168f2968
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
      "author_id": 940,
      "chapter_id": 181,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:39.869Z",
      "created_at": "2016-11-09T13:24:39.869Z",
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
      "author_id": 943,
      "chapter_id": 182,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:40.018Z",
      "created_at": "2016-11-09T13:24:40.018Z",
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
      "author_id": 946,
      "chapter_id": 183,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:40.171Z",
      "created_at": "2016-11-09T13:24:40.171Z",
      "tags": [

      ],
      "status": "reported",
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
      "author_id": 934,
      "chapter_id": 179,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:39.527Z",
      "created_at": "2016-11-09T13:24:39.527Z",
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
      "author_id": 937,
      "chapter_id": 180,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:39.720Z",
      "created_at": "2016-11-09T13:24:39.720Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8b29ecc1979e88fbc8c29015117234aa41bd030cbe9ca4893d78d0f168f2968"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer dc86f2733f68812499c015ac457e607be0d5d9016c18e3f79255a3d711160fa3
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
      "id": 84,
      "obfuscated_id": "Hu6DTUHzhWo",
      "author_id": 930,
      "chapter_id": 178,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:39.241Z",
      "created_at": "2016-11-09T13:24:39.241Z",
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
	-H "Authorization: Bearer dc86f2733f68812499c015ac457e607be0d5d9016c18e3f79255a3d711160fa3"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/92/republish
Content-Type: application/json
Authorization: Bearer 5b3f4e293c837f119c292a24adae58d0932193e9f6abc314b4b593b5aa1c613f
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/92/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b3f4e293c837f119c292a24adae58d0932193e9f6abc314b4b593b5aa1c613f"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/93/feedbacks
Content-Type: application/json
Authorization: Bearer 763d23c5a6dac387f9e8eb077daf01ecc3b979a45b3c2ba58372f9276980d012
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
      "user_id": 464,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:03.257Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 463,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:03.245Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/93/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 763d23c5a6dac387f9e8eb077daf01ecc3b979a45b3c2ba58372f9276980d012"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer c9ddb53e85b491b3325001808c84583a0716f010fb4e7661532fda95ec65ef2c
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 74,
      "chapter_id": 24,
      "position": 15,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:24.833Z",
      "created_at": "2016-11-09T13:23:24.701Z",
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 65,
      "chapter_id": 21,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:23.929Z",
      "created_at": "2016-11-09T13:23:23.802Z",
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
          "id": 42,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 43,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 68,
      "chapter_id": 22,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:24.214Z",
      "created_at": "2016-11-09T13:23:24.089Z",
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
          "id": 44,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 45,
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
      "author_id": 71,
      "chapter_id": 23,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:24.533Z",
      "created_at": "2016-11-09T13:23:24.408Z",
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
    },
    {
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 77,
      "chapter_id": 25,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:25.128Z",
      "created_at": "2016-11-09T13:23:25.004Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9ddb53e85b491b3325001808c84583a0716f010fb4e7661532fda95ec65ef2c"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 4a69fe59362581a5819b087670ca8bcabe97c00f16e893f5102926bf51dfcaa0
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 61,
      "chapter_id": 20,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:23.592Z",
      "created_at": "2016-11-09T13:23:23.479Z",
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
          "id": 40,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 41,
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
	-H "Authorization: Bearer 4a69fe59362581a5819b087670ca8bcabe97c00f16e893f5102926bf51dfcaa0"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/5/republish
Content-Type: application/json
Authorization: Bearer 1ea8abc0bc7e516ddb3c5825384607cfe6b20e9b10deecd5077ee67f39863285
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ea8abc0bc7e516ddb3c5825384607cfe6b20e9b10deecd5077ee67f39863285"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 200e3a1e65d13b34272c9290ef74c7a4bd3ccafe9b1f6e0f0ff025f77cb29ca0
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":251,"published":false}}
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
    "creator_id": 749,
    "id": 239,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 223,
    "additional_university_ids": [

    ],
    "discipline_id": 252,
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
    "updated_at": "2016-11-09T13:24:26.662Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 251,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":251,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 200e3a1e65d13b34272c9290ef74c7a4bd3ccafe9b1f6e0f0ff025f77cb29ca0"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9557f0bd5dae1172ac6c675fd10a6f30e06cc2a4e904a4759f439ecbcbe09cad
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
      "creator_id": 728,
      "id": 222,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 216,
      "additional_university_ids": [

      ],
      "discipline_id": 235,
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
      "updated_at": "2016-11-09T13:24:24.738Z",
      "shortname": "fu-course-167",
      "topic_id": 234,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 728,
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 216,
      "additional_university_ids": [

      ],
      "discipline_id": 236,
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
      "updated_at": "2016-11-09T13:24:24.777Z",
      "shortname": "fu-course-168",
      "topic_id": 235,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 729,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 216,
      "additional_university_ids": [

      ],
      "discipline_id": 237,
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
      "updated_at": "2016-11-09T13:24:24.827Z",
      "shortname": "fu-course-169",
      "topic_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 729,
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-170",
      "html_url": "https://goskive.com/course/fu-course-170",
      "slug": "fu-course-170",
      "university_id": 216,
      "additional_university_ids": [

      ],
      "discipline_id": 238,
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
      "chapters_updated_at": "2016-11-09T13:24:24.679Z",
      "updated_at": "2016-11-09T13:24:25.125Z",
      "shortname": "fu-course-170",
      "topic_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 170",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9557f0bd5dae1172ac6c675fd10a6f30e06cc2a4e904a4759f439ecbcbe09cad"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a06343b46e22d7f63978b0b6e4a2b264514cfea4a35454445630bb7488d6b881
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
      "creator_id": 734,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-171",
      "html_url": "https://goskive.com/course/fu-course-171",
      "slug": "fu-course-171",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "discipline_id": 239,
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
      "updated_at": "2016-11-09T13:24:25.268Z",
      "shortname": "fu-course-171",
      "topic_id": 238,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 171",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 734,
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "discipline_id": 240,
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
      "updated_at": "2016-11-09T13:24:25.307Z",
      "shortname": "fu-course-172",
      "topic_id": 239,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 172",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 735,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-173",
      "html_url": "https://goskive.com/course/fu-course-173",
      "slug": "fu-course-173",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "discipline_id": 241,
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
      "updated_at": "2016-11-09T13:24:25.351Z",
      "shortname": "fu-course-173",
      "topic_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 735,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-174",
      "html_url": "https://goskive.com/course/fu-course-174",
      "slug": "fu-course-174",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "discipline_id": 242,
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
      "updated_at": "2016-11-09T13:24:25.389Z",
      "shortname": "fu-course-174",
      "topic_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 174",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a06343b46e22d7f63978b0b6e4a2b264514cfea4a35454445630bb7488d6b881"
```
