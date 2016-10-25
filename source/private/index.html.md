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
DELETE /v2/chapters/6
Content-Type: application/json
Authorization: Bearer b7e33bc9504743e8f17b18b755a2dacf5e93cb80cf76aa9df3b6b19f8c977688
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7e33bc9504743e8f17b18b755a2dacf5e93cb80cf76aa9df3b6b19f8c977688"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/1
Content-Type: application/json
Authorization: Bearer 177b6e5bac00e72639745fabb6da0cc7e1bd71e26e492b3533e7562bebd096d3
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
    "updated_at": "2016-10-25T10:03:28.621Z",
    "course_id": 6,
    "author_id": 13,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T10:03:27.900Z",
    "questions_updated_at": "2016-10-25T10:03:27.900Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 16,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:28.563Z",
        "created_at": "2016-10-25T10:03:28.563Z",
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
        "author_id": 17,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:28.601Z",
        "created_at": "2016-10-25T10:03:28.601Z",
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
        "author_id": 14,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:28.273Z",
        "created_at": "2016-10-25T10:03:28.149Z",
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
        "author_id": 15,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:28.478Z",
        "created_at": "2016-10-25T10:03:28.352Z",
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
	-H "Authorization: Bearer 177b6e5bac00e72639745fabb6da0cc7e1bd71e26e492b3533e7562bebd096d3"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/3
Content-Type: application/json
Authorization: Bearer 9b298f058ffcdec6d066d88a6dfeab86bf8b76fb42383cf9a8a40d44696adec8
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
    "id": 3,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T10:03:29.577Z",
    "course_id": 8,
    "author_id": 27,
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
curl "api.goskive.com/v2/chapters/3" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b298f058ffcdec6d066d88a6dfeab86bf8b76fb42383cf9a8a40d44696adec8"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/56
Content-Type: application/json
Authorization: Bearer a2377e88b72deac2fafe9f35980e893b96ffd9e9e4830483ff703f1962501493
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2377e88b72deac2fafe9f35980e893b96ffd9e9e4830483ff703f1962501493"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 31426c900780eaae1be12c282ea4f7d57a8ffd2de48c8a65eaa9cf611c282f1b
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
      "author_id": 778,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:41.009Z",
      "status": "published",
      "subject_id": 249,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 780,
      "reply_to_id": 31,
      "created_at": "2016-10-25T10:04:41.099Z",
      "status": "published",
      "subject_id": 250,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 782,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:41.189Z",
      "status": "published",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 784,
      "reply_to_id": 33,
      "created_at": "2016-10-25T10:04:41.277Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 786,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:41.367Z",
      "status": "reported",
      "subject_id": 253,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 788,
      "reply_to_id": 35,
      "created_at": "2016-10-25T10:04:41.457Z",
      "status": "published",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 790,
      "reply_to_id": 35,
      "created_at": "2016-10-25T10:04:41.550Z",
      "status": "published",
      "subject_id": 255,
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
	-H "Authorization: Bearer 31426c900780eaae1be12c282ea4f7d57a8ffd2de48c8a65eaa9cf611c282f1b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5d6334cb133a62615b65638fc204f8b78e9649cc2ebefc5d1b21dedbc94bdb50
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
      "id": 38,
      "author_id": 793,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:41.719Z",
      "status": "published",
      "subject_id": 256,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 795,
      "reply_to_id": 38,
      "created_at": "2016-10-25T10:04:41.814Z",
      "status": "published",
      "subject_id": 257,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 797,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:41.904Z",
      "status": "published",
      "subject_id": 258,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 799,
      "reply_to_id": 40,
      "created_at": "2016-10-25T10:04:41.998Z",
      "status": "published",
      "subject_id": 259,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 801,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:42.091Z",
      "status": "reported",
      "subject_id": 260,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 803,
      "reply_to_id": 42,
      "created_at": "2016-10-25T10:04:42.182Z",
      "status": "published",
      "subject_id": 261,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 805,
      "reply_to_id": 42,
      "created_at": "2016-10-25T10:04:42.274Z",
      "status": "published",
      "subject_id": 262,
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
	-H "Authorization: Bearer 5d6334cb133a62615b65638fc204f8b78e9649cc2ebefc5d1b21dedbc94bdb50"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 19fa54dcc79b81b5d742a3d216163e6173b99f444d770e15062fb2dacdde3f97
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
      "id": 25,
      "author_id": 765,
      "reply_to_id": 24,
      "created_at": "2016-10-25T10:04:40.392Z",
      "status": "published",
      "subject_id": 243,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 769,
      "reply_to_id": 26,
      "created_at": "2016-10-25T10:04:40.567Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 773,
      "reply_to_id": 28,
      "created_at": "2016-10-25T10:04:40.752Z",
      "status": "published",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 775,
      "reply_to_id": 28,
      "created_at": "2016-10-25T10:04:40.845Z",
      "status": "published",
      "subject_id": 248,
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
	-H "Authorization: Bearer 19fa54dcc79b81b5d742a3d216163e6173b99f444d770e15062fb2dacdde3f97"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 88579c075078e7bdf087841c0daf8a270535f0b7c08087659e926d0852bce737
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
      "id": 49,
      "author_id": 816,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:42.828Z",
      "status": "reported",
      "subject_id": 267,
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
	-H "Authorization: Bearer 88579c075078e7bdf087841c0daf8a270535f0b7c08087659e926d0852bce737"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/52/republish
Content-Type: application/json
Authorization: Bearer 18e54634f54c028221aaf71ed7eb12dbb0a5c0434e9d49a799d3c9dd926b3531
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18e54634f54c028221aaf71ed7eb12dbb0a5c0434e9d49a799d3c9dd926b3531"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a97c5ecfc352b15f11d4dcb26c322fd0d6aec94d287de040b25487b309cd9573
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
    "id": 160,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T10:04:43.945Z",
    "course_id": 276,
    "author_id": 839,
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
	-H "Authorization: Bearer a97c5ecfc352b15f11d4dcb26c322fd0d6aec94d287de040b25487b309cd9573"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/279/chapters
Content-Type: application/json
Authorization: Bearer ccdd85398650d489467c6fd188beafbb4c419170ed829910042dc6601e1e0ce7
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
    "id": 162,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T10:04:44.339Z",
    "course_id": 279,
    "author_id": 845,
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
curl "api.goskive.com/v2/courses/279/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccdd85398650d489467c6fd188beafbb4c419170ed829910042dc6601e1e0ce7"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5c1f21ffec87a117c04b0395b014f28ebf6ce72e009f8d7b2f18c12899122033
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
      "id": 163,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-25T10:04:44.455Z",
      "course_id": 280,
      "author_id": 847,
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
      "id": 164,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-25T10:04:44.482Z",
      "course_id": 280,
      "author_id": 848,
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
      "id": 165,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-25T10:04:44.755Z",
      "course_id": 280,
      "author_id": 849,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T10:04:44.374Z",
      "questions_updated_at": "2016-10-25T10:04:44.374Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c1f21ffec87a117c04b0395b014f28ebf6ce72e009f8d7b2f18c12899122033"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c7fa858c6c7a3715ec99376645e4e268f9eaaefc01099afc33b8778ad5356ed1
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
      "id": 166,
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-25T10:04:44.921Z",
      "course_id": 281,
      "author_id": 854,
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
      "id": 167,
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-25T10:04:44.946Z",
      "course_id": 281,
      "author_id": 855,
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
      "id": 168,
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-25T10:04:44.972Z",
      "course_id": 281,
      "author_id": 856,
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
	-H "Authorization: Bearer c7fa858c6c7a3715ec99376645e4e268f9eaaefc01099afc33b8778ad5356ed1"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/123
Content-Type: application/json
Authorization: Bearer 2cf1d54723d987b894ad0e1d1757a600201a2fc516a048c5adb41c342c07dbc1
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/123" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cf1d54723d987b894ad0e1d1757a600201a2fc516a048c5adb41c342c07dbc1"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9073745e6f5cc8a69ee3a4d32bee341f1616a4dcaff047d3803a0afc5f1a1e3a
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
	-H "Authorization: Bearer 9073745e6f5cc8a69ee3a4d32bee341f1616a4dcaff047d3803a0afc5f1a1e3a"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b12b3caf3c4a64374c985c16703f13403ef5067ed80eb5e9fd50fe18bfbe9496
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
    "creator_id": 314,
    "id": 115,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 99,
    "additional_university_ids": [

    ],
    "topic_id": 115,
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
    "chapters_updated_at": "2016-10-25T10:04:00.863Z",
    "updated_at": "2016-10-25T10:04:02.852Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 65,
        "title": "Clever Chapter Title 50",
        "position": 1,
        "updated_at": "2016-10-25T10:04:02.793Z",
        "course_id": 115,
        "author_id": 314,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T10:04:00.863Z",
        "questions_updated_at": "2016-10-25T10:04:00.863Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 66,
        "title": "Clever Chapter Title 51",
        "position": 2,
        "updated_at": "2016-10-25T10:04:02.842Z",
        "course_id": 115,
        "author_id": 314,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T10:04:00.863Z",
        "questions_updated_at": "2016-10-25T10:04:00.863Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 314,
        "chapter_id": 65,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.560Z",
        "created_at": "2016-10-25T10:04:02.560Z",
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
        "author_id": 314,
        "chapter_id": 66,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.662Z",
        "created_at": "2016-10-25T10:04:02.662Z",
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
        "author_id": 314,
        "chapter_id": 65,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.615Z",
        "created_at": "2016-10-25T10:04:02.615Z",
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
        "author_id": 314,
        "chapter_id": 66,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.721Z",
        "created_at": "2016-10-25T10:04:02.721Z",
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
        "author_id": 317,
        "chapter_id": 65,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.778Z",
        "created_at": "2016-10-25T10:04:02.778Z",
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
        "author_id": 318,
        "chapter_id": 66,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:02.829Z",
        "created_at": "2016-10-25T10:04:02.829Z",
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
	-H "Authorization: Bearer b12b3caf3c4a64374c985c16703f13403ef5067ed80eb5e9fd50fe18bfbe9496"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/119
Content-Type: application/json
Authorization: Bearer c3a8a5ef0ebddd32a1c710b602b1c5a177e1590e1ea814ef17b0514d9d70b26b
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
    "creator_id": 333,
    "id": 119,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 119,
    "discipline_id": 119,
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
    "updated_at": "2016-10-25T10:04:07.580Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/119" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3a8a5ef0ebddd32a1c710b602b1c5a177e1590e1ea814ef17b0514d9d70b26b"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 08e91c3d0ec0c7a52c45a7640c379057fdc904a3c3e20b083ba8725ee8b26dde
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
    "creator_id": 338,
    "id": 122,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 106,
    "additional_university_ids": [

    ],
    "topic_id": 122,
    "discipline_id": 122,
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
    "updated_at": "2016-10-25T10:04:08.014Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08e91c3d0ec0c7a52c45a7640c379057fdc904a3c3e20b083ba8725ee8b26dde"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer e8067d8dbb272f7e7c4d4b16eb6c6ac8fdfceaa6760ea9d72eab4644a86a5666
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
      "id": 28,
      "user_id": 667,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:33.326Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 671,
      "feedbackable_id": 101,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:33.641Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 675,
      "feedbackable_id": 102,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:34.009Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 679,
      "feedbackable_id": 103,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:34.354Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 683,
      "feedbackable_id": 104,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T10:04:34.704Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8067d8dbb272f7e7c4d4b16eb6c6ac8fdfceaa6760ea9d72eab4644a86a5666"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 98e698a915a88674bb896066d73b4980c3a88c07a3bd78d270c4f5906dc8e3d6
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
      "id": 46,
      "user_id": 741,
      "feedbackable_id": 118,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T10:04:39.258Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98e698a915a88674bb896066d73b4980c3a88c07a3bd78d270c4f5906dc8e3d6"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer 8ec7b16ea67fa6e7335097b00ef353968abc2f0f2b2cd72b8d5ed050fe764153
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ec7b16ea67fa6e7335097b00ef353968abc2f0f2b2cd72b8d5ed050fe764153"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Content-Type: application/json
Authorization: Bearer 70c325666e6eb7b47d30c73ddc83234721a9ec74c67565e20055b9a75f16af7f
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
    "id": 5,
    "uploader": {
      "id": 561,
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
      "created_at": "2016-10-25T10:04:25.905Z",
      "updated_at": "2016-10-25T10:04:25.905Z"
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
    "created_at": "2016-10-25T10:04:25.983Z",
    "updated_at": "2016-10-25T10:04:25.983Z",
    "course_id": 191,
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
curl "api.goskive.com/v2/files/5/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70c325666e6eb7b47d30c73ddc83234721a9ec74c67565e20055b9a75f16af7f"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/80/feedbacks
Content-Type: application/json
Authorization: Bearer 86191b08c7548384bb1c01e02e7d62d5c0b85a5d9602f07fec635c84e5f95f1d
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
      "user_id": 532,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:23.662Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 531,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:23.650Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/80/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86191b08c7548384bb1c01e02e7d62d5c0b85a5d9602f07fec635c84e5f95f1d"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 2eb1f50c172743f05ea6e8f7de7dd35dd0752dba55a97ed71bbca18bb63585db
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 451,
      "chapter_id": 96,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:19.248Z",
      "created_at": "2016-10-25T10:04:19.248Z",
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
      "author_id": 454,
      "chapter_id": 97,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:19.386Z",
      "created_at": "2016-10-25T10:04:19.386Z",
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
      "author_id": 457,
      "chapter_id": 98,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:19.523Z",
      "created_at": "2016-10-25T10:04:19.523Z",
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
      "author_id": 460,
      "chapter_id": 99,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:19.657Z",
      "created_at": "2016-10-25T10:04:19.657Z",
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 463,
      "chapter_id": 100,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:19.796Z",
      "created_at": "2016-10-25T10:04:19.796Z",
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
	-H "Authorization: Bearer 2eb1f50c172743f05ea6e8f7de7dd35dd0752dba55a97ed71bbca18bb63585db"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4f8597d12371bc742c703c1cd3c30be09885330f54ea0ca1a4df9bca54096dad
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 479,
      "chapter_id": 105,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:20.585Z",
      "created_at": "2016-10-25T10:04:20.585Z",
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
	-H "Authorization: Bearer 4f8597d12371bc742c703c1cd3c30be09885330f54ea0ca1a4df9bca54096dad"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/54/republish
Content-Type: application/json
Authorization: Bearer 66516c822ca68c7bd1e3a9fe9f33e5241969247ac799625d88d7b5a526d7ee13
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66516c822ca68c7bd1e3a9fe9f33e5241969247ac799625d88d7b5a526d7ee13"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/96/feedbacks
Content-Type: application/json
Authorization: Bearer 9ef31e77ff52e3f379f652a2249d2547847829eae7b87ffa0a857a1b26488e61
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
      "id": 16,
      "user_id": 599,
      "feedbackable_id": 96,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:29.202Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 598,
      "feedbackable_id": 96,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:29.191Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/96/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ef31e77ff52e3f379f652a2249d2547847829eae7b87ffa0a857a1b26488e61"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 27d5daf55db6d4dd2ee0cb809c4ee9abd94921c608399305322c044635e3feb9
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
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 265,
      "chapter_id": 51,
      "position": 36,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:53.973Z",
      "created_at": "2016-10-25T10:03:53.822Z",
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
          "id": 85,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 86,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 256,
      "chapter_id": 48,
      "position": 33,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:52.979Z",
      "created_at": "2016-10-25T10:03:52.825Z",
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
          "id": 79,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 80,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 259,
      "chapter_id": 49,
      "position": 34,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:53.307Z",
      "created_at": "2016-10-25T10:03:53.158Z",
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
          "id": 81,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 82,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 262,
      "chapter_id": 50,
      "position": 35,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:53.641Z",
      "created_at": "2016-10-25T10:03:53.492Z",
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
          "id": 83,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 84,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 268,
      "chapter_id": 52,
      "position": 37,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:54.293Z",
      "created_at": "2016-10-25T10:03:54.152Z",
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
          "id": 87,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 88,
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
	-H "Authorization: Bearer 27d5daf55db6d4dd2ee0cb809c4ee9abd94921c608399305322c044635e3feb9"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 41a2a932395bbcebf7603f8d8e8d2af8860b759862ad316c82b815ccbb85dc95
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 284,
      "chapter_id": 57,
      "position": 42,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:56.031Z",
      "created_at": "2016-10-25T10:03:55.886Z",
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
          "id": 97,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 98,
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
	-H "Authorization: Bearer 41a2a932395bbcebf7603f8d8e8d2af8860b759862ad316c82b815ccbb85dc95"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/27/republish
Content-Type: application/json
Authorization: Bearer 9d7b4906cefae10d88c2c1fc0f9863f906c725dcdec2ce77f665dc5deee7fc0c
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d7b4906cefae10d88c2c1fc0f9863f906c725dcdec2ce77f665dc5deee7fc0c"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3212a3911dbba6af93fa9222aa72d9ed5029c956f1eb611344ad668e49473555
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":82,"published":false}}
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
    "creator_id": 209,
    "id": 82,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 66,
    "additional_university_ids": [

    ],
    "topic_id": 82,
    "discipline_id": 82,
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
    "updated_at": "2016-10-25T10:03:47.173Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":82,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3212a3911dbba6af93fa9222aa72d9ed5029c956f1eb611344ad668e49473555"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d510174ae2be0a1aa6b40b8943640e3f3058eb1a661259617a22aa0f5a496315
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
      "creator_id": 198,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "topic_id": 73,
      "discipline_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
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
      "updated_at": "2016-10-25T10:03:46.117Z",
      "shortname": "fu-course-41"
    },
    {
      "creator_id": 198,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
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
      "updated_at": "2016-10-25T10:03:46.158Z",
      "shortname": "fu-course-42"
    },
    {
      "creator_id": 199,
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-43",
      "html_url": "https://goskive.com/course/fu-course-43",
      "slug": "fu-course-43",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 43",
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
      "updated_at": "2016-10-25T10:03:46.208Z",
      "shortname": "fu-course-43"
    },
    {
      "creator_id": 199,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 76,
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
      "chapters_updated_at": "2016-10-25T10:03:46.527Z",
      "updated_at": "2016-10-25T10:03:46.534Z",
      "shortname": "fu-course-44"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d510174ae2be0a1aa6b40b8943640e3f3058eb1a661259617a22aa0f5a496315"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer eeef494854ec9f164259a5f271801c67db17dfae3b3a5f02be99154476f0e412
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
      "creator_id": 204,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 63,
      "additional_university_ids": [

      ],
      "topic_id": 77,
      "discipline_id": 77,
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
      "updated_at": "2016-10-25T10:03:46.682Z",
      "shortname": "fu-course-45"
    },
    {
      "creator_id": 204,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 63,
      "additional_university_ids": [

      ],
      "topic_id": 78,
      "discipline_id": 78,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T10:03:46.721Z",
      "shortname": "fu-course-46"
    },
    {
      "creator_id": 205,
      "id": 79,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 63,
      "additional_university_ids": [

      ],
      "topic_id": 79,
      "discipline_id": 79,
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
      "updated_at": "2016-10-25T10:03:46.769Z",
      "shortname": "fu-course-47"
    },
    {
      "creator_id": 205,
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-48",
      "html_url": "https://goskive.com/course/fu-course-48",
      "slug": "fu-course-48",
      "university_id": 63,
      "additional_university_ids": [

      ],
      "topic_id": 80,
      "discipline_id": 80,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T10:03:46.809Z",
      "shortname": "fu-course-48"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eeef494854ec9f164259a5f271801c67db17dfae3b3a5f02be99154476f0e412"
```
