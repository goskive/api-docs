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
DELETE /v2/chapters/146
Content-Type: application/json
Authorization: Bearer 32f8bfd62b9bf8613ac22f4fad691319f881d027dfdbdde0de233e5b6fd89969
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/146" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32f8bfd62b9bf8613ac22f4fad691319f881d027dfdbdde0de233e5b6fd89969"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/148
Content-Type: application/json
Authorization: Bearer 5f70705c92752a4f2f11d0b45b5315823bf36fec275ebed4de5767cd5ae9c572
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
    "id": 148,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T11:09:12.304Z",
    "course_id": 191,
    "author_id": 596,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T11:09:11.706Z",
    "questions_updated_at": "2016-10-18T11:09:11.706Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 599,
        "chapter_id": 148,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:12.242Z",
        "created_at": "2016-10-18T11:09:12.242Z",
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
        "author_id": 600,
        "chapter_id": 148,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:12.284Z",
        "created_at": "2016-10-18T11:09:12.284Z",
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
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 597,
        "chapter_id": 148,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:11.947Z",
        "created_at": "2016-10-18T11:09:11.822Z",
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
            "id": 229,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 230,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 114,
        "obfuscated_id": "RwCVsRO9fcs",
        "author_id": 598,
        "chapter_id": 148,
        "position": 101,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:12.165Z",
        "created_at": "2016-10-18T11:09:12.030Z",
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
            "id": 231,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 232,
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
curl "api.goskive.com/v2/chapters/148" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f70705c92752a4f2f11d0b45b5315823bf36fec275ebed4de5767cd5ae9c572"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/140
Content-Type: application/json
Authorization: Bearer ec7fc4659067045448bb6255ab4c17c6d822c53886c58b562ad716de23a020c4
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
    "id": 140,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T11:09:09.732Z",
    "course_id": 183,
    "author_id": 569,
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
curl "api.goskive.com/v2/chapters/140" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec7fc4659067045448bb6255ab4c17c6d822c53886c58b562ad716de23a020c4"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/59
Content-Type: application/json
Authorization: Bearer b5c5574e1eca412cc3794a804760bcb48a8896fcf9a1a335fdd0ffd8fd199b21
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5c5574e1eca412cc3794a804760bcb48a8896fcf9a1a335fdd0ffd8fd199b21"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 3d6ac6dda33f395c82ab13b3b77eb12309520786eec1abe38144ac825ae78edd
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
      "id": 34,
      "author_id": 872,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:31.691Z",
      "status": "published",
      "subject_id": 275,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 874,
      "reply_to_id": 34,
      "created_at": "2016-10-18T11:09:31.786Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 876,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:31.879Z",
      "status": "published",
      "subject_id": 277,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 878,
      "reply_to_id": 36,
      "created_at": "2016-10-18T11:09:31.977Z",
      "status": "published",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 880,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:32.070Z",
      "status": "reported",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 882,
      "reply_to_id": 38,
      "created_at": "2016-10-18T11:09:32.168Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 884,
      "reply_to_id": 38,
      "created_at": "2016-10-18T11:09:32.301Z",
      "status": "published",
      "subject_id": 281,
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
	-H "Authorization: Bearer 3d6ac6dda33f395c82ab13b3b77eb12309520786eec1abe38144ac825ae78edd"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a9ee267c2f385e29a30b79baff0853216fe2c6bad2a761b576a2099fe3518d1a
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
      "id": 48,
      "author_id": 902,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:33.183Z",
      "status": "published",
      "subject_id": 289,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 904,
      "reply_to_id": 48,
      "created_at": "2016-10-18T11:09:33.278Z",
      "status": "published",
      "subject_id": 290,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 906,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:33.373Z",
      "status": "published",
      "subject_id": 291,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 908,
      "reply_to_id": 50,
      "created_at": "2016-10-18T11:09:33.467Z",
      "status": "published",
      "subject_id": 292,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 910,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:33.566Z",
      "status": "reported",
      "subject_id": 293,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 912,
      "reply_to_id": 52,
      "created_at": "2016-10-18T11:09:33.656Z",
      "status": "published",
      "subject_id": 294,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 54,
      "author_id": 914,
      "reply_to_id": 52,
      "created_at": "2016-10-18T11:09:33.748Z",
      "status": "published",
      "subject_id": 295,
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
	-H "Authorization: Bearer a9ee267c2f385e29a30b79baff0853216fe2c6bad2a761b576a2099fe3518d1a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer bc7b2f958060297bd7bf493d909bbbba59c8e1d28efc51c8d482f1b944b61e97
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
      "author_id": 844,
      "reply_to_id": 20,
      "created_at": "2016-10-18T11:09:30.340Z",
      "status": "published",
      "subject_id": 262,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 848,
      "reply_to_id": 22,
      "created_at": "2016-10-18T11:09:30.517Z",
      "status": "published",
      "subject_id": 264,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 852,
      "reply_to_id": 24,
      "created_at": "2016-10-18T11:09:30.713Z",
      "status": "published",
      "subject_id": 266,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 854,
      "reply_to_id": 24,
      "created_at": "2016-10-18T11:09:30.810Z",
      "status": "published",
      "subject_id": 267,
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
	-H "Authorization: Bearer bc7b2f958060297bd7bf493d909bbbba59c8e1d28efc51c8d482f1b944b61e97"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer dbd034a9b94f6b8de43193786d9bbdcd42175f59e731c6000232898d34b73701
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
      "id": 45,
      "author_id": 895,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:09:32.855Z",
      "status": "reported",
      "subject_id": 286,
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
	-H "Authorization: Bearer dbd034a9b94f6b8de43193786d9bbdcd42175f59e731c6000232898d34b73701"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/56/republish
Content-Type: application/json
Authorization: Bearer 3e636faa2da9035928b7f705d50dd3998c72a39631dab5fa4acf2a40f11e818c
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e636faa2da9035928b7f705d50dd3998c72a39631dab5fa4acf2a40f11e818c"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/111/chapters
Content-Type: application/json
Authorization: Bearer 5b824f7236d50bfa65b16bffa81a0c47d61d0e4362b28f00bc49b735605412ca
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
    "id": 67,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T11:08:42.457Z",
    "course_id": 111,
    "author_id": 291,
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
curl "api.goskive.com/v2/courses/111/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b824f7236d50bfa65b16bffa81a0c47d61d0e4362b28f00bc49b735605412ca"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d8883eb575f00b7b431a5813c05a65d08c38b6987688482f6968fefe543b93e1
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
    "id": 68,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T11:08:42.599Z",
    "course_id": 112,
    "author_id": 293,
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
	-H "Authorization: Bearer d8883eb575f00b7b431a5813c05a65d08c38b6987688482f6968fefe543b93e1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9a16c8b884fe2317cc58ad6163fbd3239383f9187b6f4e9f9f1590867cc0e5c9
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
      "id": 82,
      "title": "Clever Chapter Title 70",
      "position": 1,
      "updated_at": "2016-10-18T11:08:44.393Z",
      "course_id": 121,
      "author_id": 324,
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
      "id": 83,
      "title": "Clever Chapter Title 71",
      "position": 2,
      "updated_at": "2016-10-18T11:08:44.418Z",
      "course_id": 121,
      "author_id": 325,
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
      "id": 84,
      "title": "Clever Chapter Title 72",
      "position": 3,
      "updated_at": "2016-10-18T11:08:44.676Z",
      "course_id": 121,
      "author_id": 326,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T11:08:44.314Z",
      "questions_updated_at": "2016-10-18T11:08:44.314Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a16c8b884fe2317cc58ad6163fbd3239383f9187b6f4e9f9f1590867cc0e5c9"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b769dc73bb690114ab271330f086a9f3c94753548e3bc3973cd3d9f16bfce11e
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
      "id": 85,
      "title": "Clever Chapter Title 73",
      "position": 1,
      "updated_at": "2016-10-18T11:08:44.921Z",
      "course_id": 123,
      "author_id": 333,
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
      "id": 86,
      "title": "Clever Chapter Title 74",
      "position": 2,
      "updated_at": "2016-10-18T11:08:44.946Z",
      "course_id": 123,
      "author_id": 334,
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
      "id": 87,
      "title": "Clever Chapter Title 75",
      "position": 3,
      "updated_at": "2016-10-18T11:08:44.971Z",
      "course_id": 123,
      "author_id": 335,
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
	-H "Authorization: Bearer b769dc73bb690114ab271330f086a9f3c94753548e3bc3973cd3d9f16bfce11e"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 35268f5d85ec5abec3f20deb378492212888d83522c00736c79db450ec3e1a68
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
	-H "Authorization: Bearer 35268f5d85ec5abec3f20deb378492212888d83522c00736c79db450ec3e1a68"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/151
Content-Type: application/json
Authorization: Bearer f78c94272ac2f6da2b925a776e9bb9fcdec5f321dcfe7d3a9fd174b439e04100
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/151" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f78c94272ac2f6da2b925a776e9bb9fcdec5f321dcfe7d3a9fd174b439e04100"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 1af59fbda5e43c61e5295d18707d81d8bffa06d287c01b36b30467e819f411d3
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
    "creator_id": 389,
    "id": 140,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 120,
    "additional_university_ids": [

    ],
    "topic_id": 145,
    "discipline_id": 145,
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
    "chapters_updated_at": "2016-10-18T11:08:51.168Z",
    "updated_at": "2016-10-18T11:08:52.768Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 101,
        "title": "Clever Chapter Title 89",
        "position": 1,
        "updated_at": "2016-10-18T11:08:52.715Z",
        "course_id": 140,
        "author_id": 389,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T11:08:51.168Z",
        "questions_updated_at": "2016-10-18T11:08:51.168Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 102,
        "title": "Clever Chapter Title 90",
        "position": 2,
        "updated_at": "2016-10-18T11:08:52.759Z",
        "course_id": 140,
        "author_id": 389,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T11:08:51.168Z",
        "questions_updated_at": "2016-10-18T11:08:51.168Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 389,
        "chapter_id": 101,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.535Z",
        "created_at": "2016-10-18T11:08:52.535Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 389,
        "chapter_id": 102,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.616Z",
        "created_at": "2016-10-18T11:08:52.616Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 389,
        "chapter_id": 101,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.581Z",
        "created_at": "2016-10-18T11:08:52.581Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 389,
        "chapter_id": 102,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.662Z",
        "created_at": "2016-10-18T11:08:52.662Z",
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
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 392,
        "chapter_id": 101,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.704Z",
        "created_at": "2016-10-18T11:08:52.704Z",
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
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 393,
        "chapter_id": 102,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:52.748Z",
        "created_at": "2016-10-18T11:08:52.748Z",
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
	-H "Authorization: Bearer 1af59fbda5e43c61e5295d18707d81d8bffa06d287c01b36b30467e819f411d3"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/138
Content-Type: application/json
Authorization: Bearer ac04effcb8783906acd4a557cf8d0c719acfa5d5307634790a678aa88c47e4a0
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
    "creator_id": 381,
    "id": 138,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 118,
    "additional_university_ids": [

    ],
    "topic_id": 143,
    "discipline_id": 143,
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
    "updated_at": "2016-10-18T11:08:49.400Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/138" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac04effcb8783906acd4a557cf8d0c719acfa5d5307634790a678aa88c47e4a0"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0ea897ae5e2746a218e35cc3db25f967bb3cd2151165e93c15fb08b2a4c2da6d
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
    "creator_id": 376,
    "id": 135,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "topic_id": 140,
    "discipline_id": 140,
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
    "updated_at": "2016-10-18T11:08:49.023Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ea897ae5e2746a218e35cc3db25f967bb3cd2151165e93c15fb08b2a4c2da6d"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 7d62202d7ec4c3d92b5e1c3f5e71928864264240057da9cc28d0aa5d5661085f
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
      "user_id": 458,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:59.645Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 462,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:59.994Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 466,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:09:00.346Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 470,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:09:00.698Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 474,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T11:09:01.050Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d62202d7ec4c3d92b5e1c3f5e71928864264240057da9cc28d0aa5d5661085f"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 11f8df7fafe847b7c1bed1294ab4fe06af899332ddb36ad675a0f8d2afd24a2f
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
      "id": 42,
      "user_id": 532,
      "feedbackable_id": 107,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T11:09:06.208Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11f8df7fafe847b7c1bed1294ab4fe06af899332ddb36ad675a0f8d2afd24a2f"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 40a7ee881351508f1354cec542b613a44d73016fc64ae71090395a6fd4f8b68a
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
curl "api.goskive.com/v2/files/4" -d '' -X DELETE \
	-H "Authorization: Bearer 40a7ee881351508f1354cec542b613a44d73016fc64ae71090395a6fd4f8b68a" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/8/feedbacks
Content-Type: application/json
Authorization: Bearer e38bb3941b90e02c8c316bec9203f9ae52dc992769cf652c35cc20dbd374623a
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
      "id": 8,
      "user_id": 56,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:19.806Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 55,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:19.795Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e38bb3941b90e02c8c316bec9203f9ae52dc992769cf652c35cc20dbd374623a"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer a56886d29441bb463faabe402403435427ae3471043a67bef58fcc44df5b8143
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 755,
      "chapter_id": 173,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:23.434Z",
      "created_at": "2016-10-18T11:09:23.434Z",
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
      "id": 79,
      "obfuscated_id": "BFjsqYG0c2I",
      "author_id": 758,
      "chapter_id": 174,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:23.604Z",
      "created_at": "2016-10-18T11:09:23.604Z",
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
      "id": 80,
      "obfuscated_id": "94gVa2GR5x8",
      "author_id": 761,
      "chapter_id": 175,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:23.745Z",
      "created_at": "2016-10-18T11:09:23.745Z",
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
      "author_id": 764,
      "chapter_id": 176,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:23.884Z",
      "created_at": "2016-10-18T11:09:23.884Z",
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
      "author_id": 767,
      "chapter_id": 177,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:24.019Z",
      "created_at": "2016-10-18T11:09:24.019Z",
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
	-H "Authorization: Bearer a56886d29441bb463faabe402403435427ae3471043a67bef58fcc44df5b8143"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer c679577f2dce1514bf9d61d287903396ba7279a66856db875fba00c6f6620fa9
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 735,
      "chapter_id": 167,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:22.436Z",
      "created_at": "2016-10-18T11:09:22.436Z",
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
	-H "Authorization: Bearer c679577f2dce1514bf9d61d287903396ba7279a66856db875fba00c6f6620fa9"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/republish
Content-Type: application/json
Authorization: Bearer 0cfc19ce952a922015e27cfd79cc61e195e93a0a0d0b7b369da4ca2ebf2eea34
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cfc19ce952a922015e27cfd79cc61e195e93a0a0d0b7b369da4ca2ebf2eea34"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/44/feedbacks
Content-Type: application/json
Authorization: Bearer 6f99b7ebe4263dcc36b53f7a68de81e5d276738ddd921a66bacc8a1dafc0fdf5
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
      "id": 11,
      "user_id": 258,
      "feedbackable_id": 44,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:39.664Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 257,
      "feedbackable_id": 44,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:39.653Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/44/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f99b7ebe4263dcc36b53f7a68de81e5d276738ddd921a66bacc8a1dafc0fdf5"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 41a9aece5bc0413da488fd8673009fcb3aa2ee6092301c6d83d8fa5449a4ef89
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 99,
      "chapter_id": 22,
      "position": 5,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:25.017Z",
      "created_at": "2016-10-18T11:08:24.900Z",
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
          "id": 28,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 29,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 90,
      "chapter_id": 19,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:24.154Z",
      "created_at": "2016-10-18T11:08:24.039Z",
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
          "id": 22,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 23,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 93,
      "chapter_id": 20,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:24.448Z",
      "created_at": "2016-10-18T11:08:24.325Z",
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
          "id": 24,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 25,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 96,
      "chapter_id": 21,
      "position": 4,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:24.734Z",
      "created_at": "2016-10-18T11:08:24.616Z",
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
          "id": 26,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 27,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 102,
      "chapter_id": 23,
      "position": 6,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:25.298Z",
      "created_at": "2016-10-18T11:08:25.184Z",
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
          "id": 30,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 31,
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
	-H "Authorization: Bearer 41a9aece5bc0413da488fd8673009fcb3aa2ee6092301c6d83d8fa5449a4ef89"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 0e32676304d867ec65b0d1b8cb11189fe7dd25197b26cfd8e3ffe37430a8ac3e
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 134,
      "chapter_id": 33,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:28.282Z",
      "created_at": "2016-10-18T11:08:28.170Z",
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
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e32676304d867ec65b0d1b8cb11189fe7dd25197b26cfd8e3ffe37430a8ac3e"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/9/republish
Content-Type: application/json
Authorization: Bearer ed74ab957b726b90494a846bd1ea4944769d738b9a1ad6fd184b96b59928a97f
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/9/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed74ab957b726b90494a846bd1ea4944769d738b9a1ad6fd184b96b59928a97f"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d36a0fcd6422930210bb3562dd617e0a7de14233476352c0ad28afde724b57f5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":67,"published":false}}
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
    "creator_id": 211,
    "id": 65,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 67,
    "additional_university_ids": [

    ],
    "topic_id": 67,
    "discipline_id": 67,
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
    "updated_at": "2016-10-18T11:08:35.574Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":67,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d36a0fcd6422930210bb3562dd617e0a7de14233476352c0ad28afde724b57f5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer baf85556d1454316c0adcffc29f3870fe911b5015767332a150751f2d3274496
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
      "creator_id": 217,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "topic_id": 73,
      "discipline_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
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
      "updated_at": "2016-10-18T11:08:36.084Z",
      "shortname": "fu-course-57"
    },
    {
      "creator_id": 217,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
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
      "updated_at": "2016-10-18T11:08:36.121Z",
      "shortname": "fu-course-58"
    },
    {
      "creator_id": 218,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 59",
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
      "updated_at": "2016-10-18T11:08:36.168Z",
      "shortname": "fu-course-59"
    },
    {
      "creator_id": 218,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-60",
      "html_url": "https://goskive.com/course/fu-course-60",
      "slug": "fu-course-60",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 76,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 60",
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
      "chapters_updated_at": "2016-10-18T11:08:36.456Z",
      "updated_at": "2016-10-18T11:08:36.462Z",
      "shortname": "fu-course-60"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer baf85556d1454316c0adcffc29f3870fe911b5015767332a150751f2d3274496"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9369d289bca2bbaf548990188db2975a08d901e8e2f380144084ff3acbdb9002
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
      "creator_id": 223,
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-61",
      "html_url": "https://goskive.com/course/fu-course-61",
      "slug": "fu-course-61",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 77,
      "discipline_id": 77,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
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
      "updated_at": "2016-10-18T11:08:36.610Z",
      "shortname": "fu-course-61"
    },
    {
      "creator_id": 223,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-62",
      "html_url": "https://goskive.com/course/fu-course-62",
      "slug": "fu-course-62",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 78,
      "discipline_id": 78,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 62",
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
      "updated_at": "2016-10-18T11:08:36.649Z",
      "shortname": "fu-course-62"
    },
    {
      "creator_id": 224,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-63",
      "html_url": "https://goskive.com/course/fu-course-63",
      "slug": "fu-course-63",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 79,
      "discipline_id": 79,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 63",
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
      "updated_at": "2016-10-18T11:08:36.696Z",
      "shortname": "fu-course-63"
    },
    {
      "creator_id": 224,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-64",
      "html_url": "https://goskive.com/course/fu-course-64",
      "slug": "fu-course-64",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 80,
      "discipline_id": 80,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 64",
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
      "updated_at": "2016-10-18T11:08:36.735Z",
      "shortname": "fu-course-64"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9369d289bca2bbaf548990188db2975a08d901e8e2f380144084ff3acbdb9002"
```
