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
DELETE /v2/chapters/12
Content-Type: application/json
Authorization: Bearer 434d672e7860685fec548315e9c8d83f4eb91a88c20c4be83843ce292e24c2b7
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 434d672e7860685fec548315e9c8d83f4eb91a88c20c4be83843ce292e24c2b7"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/10
Content-Type: application/json
Authorization: Bearer 503b688a1c1139b60714dd2d895a6ecbf29045885d246125ff4762e375365fb0
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
    "id": 10,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T13:39:27.645Z",
    "course_id": 18,
    "author_id": 50,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-13T13:39:27.040Z",
    "questions_updated_at": "2016-10-13T13:39:27.040Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 53,
        "chapter_id": 10,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:27.572Z",
        "created_at": "2016-10-13T13:39:27.572Z",
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
        "author_id": 54,
        "chapter_id": 10,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:27.625Z",
        "created_at": "2016-10-13T13:39:27.625Z",
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
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 51,
        "chapter_id": 10,
        "position": 7,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:27.274Z",
        "created_at": "2016-10-13T13:39:27.152Z",
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
            "id": 13,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 14,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 52,
        "chapter_id": 10,
        "position": 8,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:27.485Z",
        "created_at": "2016-10-13T13:39:27.355Z",
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
            "id": 15,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 16,
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
curl "api.goskive.com/v2/chapters/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 503b688a1c1139b60714dd2d895a6ecbf29045885d246125ff4762e375365fb0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/8
Content-Type: application/json
Authorization: Bearer 6e4e5d184524a01cb5978ea47a0cd61d494c26b98294395576088c8ecfd644c2
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
    "id": 8,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T13:39:26.838Z",
    "course_id": 16,
    "author_id": 45,
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
curl "api.goskive.com/v2/chapters/8" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e4e5d184524a01cb5978ea47a0cd61d494c26b98294395576088c8ecfd644c2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/58
Content-Type: application/json
Authorization: Bearer 0b851131f0a52ff8439055f57f2c37ff6f1833bb3740bc5eb3a8dacc448bf131
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b851131f0a52ff8439055f57f2c37ff6f1833bb3740bc5eb3a8dacc448bf131"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 3ee4a9d0531399f06536b9d0e9c8b185e29d51d1a846002dd9a3b613592bc221
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
      "id": 20,
      "author_id": 774,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:31.198Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 776,
      "reply_to_id": 20,
      "created_at": "2016-10-13T13:40:31.288Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 778,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:31.381Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 780,
      "reply_to_id": 22,
      "created_at": "2016-10-13T13:40:31.476Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 782,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:31.570Z",
      "status": "reported",
      "subject_id": 240,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 784,
      "reply_to_id": 24,
      "created_at": "2016-10-13T13:40:31.660Z",
      "status": "published",
      "subject_id": 241,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 786,
      "reply_to_id": 24,
      "created_at": "2016-10-13T13:40:31.754Z",
      "status": "published",
      "subject_id": 242,
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
	-H "Authorization: Bearer 3ee4a9d0531399f06536b9d0e9c8b185e29d51d1a846002dd9a3b613592bc221"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2fdade4be121b4f0f0e9d5fe223597183ce89aa73afec8a8dd2eb86f7d36ed1e
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
      "id": 27,
      "author_id": 789,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:31.908Z",
      "status": "published",
      "subject_id": 243,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 791,
      "reply_to_id": 27,
      "created_at": "2016-10-13T13:40:31.995Z",
      "status": "published",
      "subject_id": 244,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 793,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:32.086Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 795,
      "reply_to_id": 29,
      "created_at": "2016-10-13T13:40:32.174Z",
      "status": "published",
      "subject_id": 246,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 797,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:32.263Z",
      "status": "reported",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 799,
      "reply_to_id": 31,
      "created_at": "2016-10-13T13:40:32.355Z",
      "status": "published",
      "subject_id": 248,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 801,
      "reply_to_id": 31,
      "created_at": "2016-10-13T13:40:32.444Z",
      "status": "published",
      "subject_id": 249,
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
	-H "Authorization: Bearer 2fdade4be121b4f0f0e9d5fe223597183ce89aa73afec8a8dd2eb86f7d36ed1e"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer f90037b84bfdb9cd6124b4f90bc28760b34a28c4e8ce5d2b5ccc2fa2358e5afd
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
      "id": 35,
      "author_id": 806,
      "reply_to_id": 34,
      "created_at": "2016-10-13T13:40:32.681Z",
      "status": "published",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 810,
      "reply_to_id": 36,
      "created_at": "2016-10-13T13:40:32.858Z",
      "status": "published",
      "subject_id": 253,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 814,
      "reply_to_id": 38,
      "created_at": "2016-10-13T13:40:33.037Z",
      "status": "published",
      "subject_id": 255,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 816,
      "reply_to_id": 38,
      "created_at": "2016-10-13T13:40:33.128Z",
      "status": "published",
      "subject_id": 256,
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
	-H "Authorization: Bearer f90037b84bfdb9cd6124b4f90bc28760b34a28c4e8ce5d2b5ccc2fa2358e5afd"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 131a2c94a583948246f90eb7ad510ab3e1a99f0024fce3ef3c63e484ece55478
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
      "id": 52,
      "author_id": 842,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:40:34.381Z",
      "status": "reported",
      "subject_id": 268,
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
	-H "Authorization: Bearer 131a2c94a583948246f90eb7ad510ab3e1a99f0024fce3ef3c63e484ece55478"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/55/republish
Content-Type: application/json
Authorization: Bearer 5694a9dfc07e1ed652aa5833fa41cd03bf33c8d9fd87193ee2f4a2b85b087f0b
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5694a9dfc07e1ed652aa5833fa41cd03bf33c8d9fd87193ee2f4a2b85b087f0b"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c58212e38c9acd8e7396db1f4dcd2ce29dcc7a2136b386b380b1d7f0ca3f4bff
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
    "id": 170,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T13:40:30.832Z",
    "course_id": 234,
    "author_id": 768,
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
	-H "Authorization: Bearer c58212e38c9acd8e7396db1f4dcd2ce29dcc7a2136b386b380b1d7f0ca3f4bff"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/235/chapters
Content-Type: application/json
Authorization: Bearer acf1fe3d6684c6a8ce7429e6557eae8653edd5c7f445b2df255b55e37e35adf1
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
    "id": 171,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T13:40:30.983Z",
    "course_id": 235,
    "author_id": 770,
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
curl "api.goskive.com/v2/courses/235/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer acf1fe3d6684c6a8ce7429e6557eae8653edd5c7f445b2df255b55e37e35adf1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b3724c6d21e18e1d464ac66f8058c109563c5a88375fdbd91cf7f8173ef48060
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-13T13:40:29.776Z",
      "course_id": 229,
      "author_id": 750,
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
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-13T13:40:29.802Z",
      "course_id": 229,
      "author_id": 751,
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
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-13T13:40:30.064Z",
      "course_id": 229,
      "author_id": 752,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-13T13:40:29.696Z",
      "questions_updated_at": "2016-10-13T13:40:29.696Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3724c6d21e18e1d464ac66f8058c109563c5a88375fdbd91cf7f8173ef48060"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f9fd0ba5eb69f750e2c2ca12a0ccfd922fb2b059705ba7aa56cc912bce9a5447
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
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-13T13:40:30.326Z",
      "course_id": 231,
      "author_id": 759,
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
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-13T13:40:30.352Z",
      "course_id": 231,
      "author_id": 760,
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
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-13T13:40:30.377Z",
      "course_id": 231,
      "author_id": 761,
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
	-H "Authorization: Bearer f9fd0ba5eb69f750e2c2ca12a0ccfd922fb2b059705ba7aa56cc912bce9a5447"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/294
Content-Type: application/json
Authorization: Bearer 42ebc8a98aa8d4fe8eb9f0582ce252d3601f1bff422658102b54607d700cc54c
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/294" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42ebc8a98aa8d4fe8eb9f0582ce252d3601f1bff422658102b54607d700cc54c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ecf75e49eb6500dc36d7ee260e8201d9ceb2487de64712ed94aaf13649b56221
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
	-H "Authorization: Bearer ecf75e49eb6500dc36d7ee260e8201d9ceb2487de64712ed94aaf13649b56221"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer e043c7ca2070a54e1eb29ab7994653c3e1fa632462239a04dcded321d938d1b4
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
    "creator_id": 923,
    "id": 291,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 276,
    "additional_university_ids": [

    ],
    "topic_id": 303,
    "discipline_id": 304,
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
    "chapters_updated_at": "2016-10-13T13:40:43.916Z",
    "updated_at": "2016-10-13T13:40:45.421Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 188,
        "title": "Clever Chapter Title 164",
        "position": 1,
        "updated_at": "2016-10-13T13:40:45.371Z",
        "course_id": 291,
        "author_id": 923,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T13:40:43.916Z",
        "questions_updated_at": "2016-10-13T13:40:43.916Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 189,
        "title": "Clever Chapter Title 165",
        "position": 2,
        "updated_at": "2016-10-13T13:40:45.413Z",
        "course_id": 291,
        "author_id": 923,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T13:40:43.916Z",
        "questions_updated_at": "2016-10-13T13:40:43.916Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 923,
        "chapter_id": 188,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.204Z",
        "created_at": "2016-10-13T13:40:45.204Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 923,
        "chapter_id": 189,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.277Z",
        "created_at": "2016-10-13T13:40:45.277Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 923,
        "chapter_id": 188,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.245Z",
        "created_at": "2016-10-13T13:40:45.245Z",
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
        "author_id": 923,
        "chapter_id": 189,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.318Z",
        "created_at": "2016-10-13T13:40:45.318Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 926,
        "chapter_id": 188,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.360Z",
        "created_at": "2016-10-13T13:40:45.360Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 927,
        "chapter_id": 189,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.402Z",
        "created_at": "2016-10-13T13:40:45.402Z",
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
	-H "Authorization: Bearer e043c7ca2070a54e1eb29ab7994653c3e1fa632462239a04dcded321d938d1b4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/304
Content-Type: application/json
Authorization: Bearer 6d775b67a7f8ac48fba70ced2869b8a9e0c978fc06b4b5ed7d0f446e64e7b777
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
    "creator_id": 958,
    "id": 304,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 289,
    "additional_university_ids": [

    ],
    "topic_id": 316,
    "discipline_id": 317,
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
    "updated_at": "2016-10-13T13:40:49.092Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/304" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d775b67a7f8ac48fba70ced2869b8a9e0c978fc06b4b5ed7d0f446e64e7b777"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 210fe84e33cce67a8745f9797cbbc9efb15acb92387448a07c21e58604dc79bb
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
    "creator_id": 963,
    "id": 307,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 292,
    "additional_university_ids": [

    ],
    "topic_id": 319,
    "discipline_id": 320,
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
    "updated_at": "2016-10-13T13:40:49.493Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 210fe84e33cce67a8745f9797cbbc9efb15acb92387448a07c21e58604dc79bb"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer d4c5688827b15a780b3ac0fd47dc8167d536cf418ce03e26650985e3577057cc
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
      "user_id": 342,
      "feedbackable_id": 24,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:48.726Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 346,
      "feedbackable_id": 25,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:49.096Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 350,
      "feedbackable_id": 26,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:49.435Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 354,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:49.781Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 358,
      "feedbackable_id": 28,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T13:39:50.123Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4c5688827b15a780b3ac0fd47dc8167d536cf418ce03e26650985e3577057cc"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 05c1ee9771ec97cd0f2fafc9f4e6195a15604869919549130ff4e4cc90b24056
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
      "user_id": 337,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T13:39:48.339Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05c1ee9771ec97cd0f2fafc9f4e6195a15604869919549130ff4e4cc90b24056"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer 6baef977f4fb767efeecd963cb15591f49eba6b5c4c981d208ca88a4655fdff1
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
	-H "Authorization: Bearer 6baef977f4fb767efeecd963cb15591f49eba6b5c4c981d208ca88a4655fdff1" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/11/feedbacks
Content-Type: application/json
Authorization: Bearer a94cd2defb73b13eacd609b538f3ce5c8d4fa660b297842d429c0242188f38a7
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
      "user_id": 118,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:32.165Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 117,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:32.151Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/11/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a94cd2defb73b13eacd609b538f3ce5c8d4fa660b297842d429c0242188f38a7"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 9dc11474bae1082ffaf9ccc0a7c7edd2110676fc2564fd94e01578d29393f48a
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 179,
      "chapter_id": 35,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:38.899Z",
      "created_at": "2016-10-13T13:39:38.899Z",
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
      "author_id": 182,
      "chapter_id": 36,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:39.047Z",
      "created_at": "2016-10-13T13:39:39.047Z",
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 185,
      "chapter_id": 37,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:39.197Z",
      "created_at": "2016-10-13T13:39:39.197Z",
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 188,
      "chapter_id": 38,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:39.346Z",
      "created_at": "2016-10-13T13:39:39.346Z",
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 191,
      "chapter_id": 39,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:39.491Z",
      "created_at": "2016-10-13T13:39:39.491Z",
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
	-H "Authorization: Bearer 9dc11474bae1082ffaf9ccc0a7c7edd2110676fc2564fd94e01578d29393f48a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 002fff0412a57e01abe4fbd9f0113f38661909535d4902007c2faad957a984ee
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 223,
      "chapter_id": 49,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:39:41.069Z",
      "created_at": "2016-10-13T13:39:41.069Z",
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
	-H "Authorization: Bearer 002fff0412a57e01abe4fbd9f0113f38661909535d4902007c2faad957a984ee"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/republish
Content-Type: application/json
Authorization: Bearer ca64f59a17f238dccc560e34a7f6ae4b3a85123b1165b2937381c006d5d9472b
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca64f59a17f238dccc560e34a7f6ae4b3a85123b1165b2937381c006d5d9472b"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/93/feedbacks
Content-Type: application/json
Authorization: Bearer cdd6abaaf8c0edaed9b55f582734abf8c82c43ca5c6e130d39c97f6fedd754e1
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
      "id": 44,
      "user_id": 706,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:40:26.550Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 705,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:40:26.538Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/93/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdd6abaaf8c0edaed9b55f582734abf8c82c43ca5c6e130d39c97f6fedd754e1"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer d056b717818bb44437062e732c0c8ae0bb483058a8155fe79edc3a5e971e41a8
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
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 529,
      "chapter_id": 106,
      "position": 54,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:06.959Z",
      "created_at": "2016-10-13T13:40:06.799Z",
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
          "id": 114,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 115,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 538,
      "chapter_id": 109,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:08.009Z",
      "created_at": "2016-10-13T13:40:07.844Z",
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
          "id": 120,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 121,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 532,
      "chapter_id": 107,
      "position": 55,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:07.310Z",
      "created_at": "2016-10-13T13:40:07.148Z",
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
          "id": 116,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 117,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 535,
      "chapter_id": 108,
      "position": 56,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:07.657Z",
      "created_at": "2016-10-13T13:40:07.496Z",
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
          "id": 118,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 119,
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
      "author_id": 541,
      "chapter_id": 110,
      "position": 58,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:08.355Z",
      "created_at": "2016-10-13T13:40:08.201Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d056b717818bb44437062e732c0c8ae0bb483058a8155fe79edc3a5e971e41a8"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer a9e860a7a4dbc4522a07285952b6f0f107498b59979726f8ea343148579daa39
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 557,
      "chapter_id": 115,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:10.222Z",
      "created_at": "2016-10-13T13:40:10.061Z",
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
          "id": 132,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 133,
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
	-H "Authorization: Bearer a9e860a7a4dbc4522a07285952b6f0f107498b59979726f8ea343148579daa39"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/74/republish
Content-Type: application/json
Authorization: Bearer 8d61590c2ecdee46955a83c55feacaacdc0e5ab6ddfb65fc1bf71635f8d912b5
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/74/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d61590c2ecdee46955a83c55feacaacdc0e5ab6ddfb65fc1bf71635f8d912b5"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d33ba71b255bf2e5dec99ae29e754fbc8040f1d8a3a3c77a051382950aa06308
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":179,"published":false}}
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
    "creator_id": 631,
    "id": 174,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "topic_id": 179,
    "discipline_id": 179,
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
    "updated_at": "2016-10-13T13:40:20.083Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":179,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d33ba71b255bf2e5dec99ae29e754fbc8040f1d8a3a3c77a051382950aa06308"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b27a9dda6cddec7d0c057dfebefa1d0598c720e5e5c7e8a77e460eef0d2865d8
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
      "creator_id": 653,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 184,
      "additional_university_ids": [

      ],
      "topic_id": 200,
      "discipline_id": 200,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T13:40:22.469Z",
      "shortname": "fu-course-162"
    },
    {
      "creator_id": 653,
      "id": 196,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 184,
      "additional_university_ids": [

      ],
      "topic_id": 201,
      "discipline_id": 201,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T13:40:22.509Z",
      "shortname": "fu-course-163"
    },
    {
      "creator_id": 654,
      "id": 197,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-164",
      "html_url": "https://goskive.com/course/fu-course-164",
      "slug": "fu-course-164",
      "university_id": 184,
      "additional_university_ids": [

      ],
      "topic_id": 202,
      "discipline_id": 202,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 164",
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
      "updated_at": "2016-10-13T13:40:22.558Z",
      "shortname": "fu-course-164"
    },
    {
      "creator_id": 654,
      "id": 198,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 184,
      "additional_university_ids": [

      ],
      "topic_id": 203,
      "discipline_id": 203,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
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
      "chapters_updated_at": "2016-10-13T13:40:22.852Z",
      "updated_at": "2016-10-13T13:40:22.859Z",
      "shortname": "fu-course-165"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b27a9dda6cddec7d0c057dfebefa1d0598c720e5e5c7e8a77e460eef0d2865d8"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b2e37f82d93867997222c3d628585ebf37cfe2d3f23d764c54ddae0c91a18a4d
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
      "creator_id": 660,
      "id": 199,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 204,
      "discipline_id": 204,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
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
      "updated_at": "2016-10-13T13:40:23.067Z",
      "shortname": "fu-course-166"
    },
    {
      "creator_id": 660,
      "id": 200,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 205,
      "discipline_id": 205,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
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
      "updated_at": "2016-10-13T13:40:23.110Z",
      "shortname": "fu-course-167"
    },
    {
      "creator_id": 661,
      "id": 201,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 206,
      "discipline_id": 206,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
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
      "updated_at": "2016-10-13T13:40:23.164Z",
      "shortname": "fu-course-168"
    },
    {
      "creator_id": 661,
      "id": 202,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 207,
      "discipline_id": 207,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
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
      "updated_at": "2016-10-13T13:40:23.206Z",
      "shortname": "fu-course-169"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2e37f82d93867997222c3d628585ebf37cfe2d3f23d764c54ddae0c91a18a4d"
```
