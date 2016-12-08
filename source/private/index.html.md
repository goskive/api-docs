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
DELETE /v2/chapters/129
Content-Type: application/json
Authorization: Bearer 4cd6df429cfc6318595efa74950737409f12b5b67696aa0195b73b6d3c9bb66d
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/129" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cd6df429cfc6318595efa74950737409f12b5b67696aa0195b73b6d3c9bb66d"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/130
Content-Type: application/json
Authorization: Bearer 8d1206ea726024ab4efe23534eccf745c356dbb0e6cae578453090c432c34984
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
    "id": 130,
    "updated_at": "2016-12-08T21:04:55.740Z",
    "course_id": 212,
    "author_id": 710,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-08T21:04:55.254Z",
    "questions_updated_at": "2016-12-08T21:04:55.254Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 713,
        "chapter_id": 130,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:55.683Z",
        "created_at": "2016-12-08T21:04:55.683Z",
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
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 714,
        "chapter_id": 130,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:55.722Z",
        "created_at": "2016-12-08T21:04:55.722Z",
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
        "id": 108,
        "obfuscated_id": "3MKez0MLRBM",
        "author_id": 711,
        "chapter_id": 130,
        "position": 95,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:55.466Z",
        "created_at": "2016-12-08T21:04:55.390Z",
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
            "id": 219,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 220,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 109,
        "obfuscated_id": "VSPyck5c2RY",
        "author_id": 712,
        "chapter_id": 130,
        "position": 96,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:55.621Z",
        "created_at": "2016-12-08T21:04:55.533Z",
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
            "id": 221,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 222,
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
curl "api.goskive.com/v2/chapters/130" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d1206ea726024ab4efe23534eccf745c356dbb0e6cae578453090c432c34984"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/134
Content-Type: application/json
Authorization: Bearer 4c3ca96855379f1a92d75d0bff37552d0e749f06a7a8ecbfb9f95141345a367a
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
    "id": 134,
    "updated_at": "2016-12-08T21:04:56.947Z",
    "course_id": 216,
    "author_id": 729,
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
curl "api.goskive.com/v2/chapters/134" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c3ca96855379f1a92d75d0bff37552d0e749f06a7a8ecbfb9f95141345a367a"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/10
Content-Type: application/json
Authorization: Bearer 576e39298133f8a9658e4fd88630f149884f734ca1e66867d473f6ec52ad1dc7
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 576e39298133f8a9658e4fd88630f149884f734ca1e66867d473f6ec52ad1dc7"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer bc10a17a5eeb2213fef6d0e3bcb9b357faf3ca8b1f3ceeb28c5c19e1f7929a4f
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
      "id": 28,
      "author_id": 529,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:43.840Z",
      "status": "published",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 531,
      "reply_to_id": 28,
      "created_at": "2016-12-08T21:04:43.947Z",
      "status": "published",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 533,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:44.055Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 535,
      "reply_to_id": 30,
      "created_at": "2016-12-08T21:04:44.161Z",
      "status": "published",
      "subject_id": 154,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 537,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:44.269Z",
      "status": "reported",
      "subject_id": 155,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 539,
      "reply_to_id": 32,
      "created_at": "2016-12-08T21:04:44.377Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 541,
      "reply_to_id": 32,
      "created_at": "2016-12-08T21:04:44.486Z",
      "status": "published",
      "subject_id": 157,
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
	-H "Authorization: Bearer bc10a17a5eeb2213fef6d0e3bcb9b357faf3ca8b1f3ceeb28c5c19e1f7929a4f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 313a00c0a72e14fbf385bf93c3b75b21efdbc8870b476eb67b5c9035c40f312e
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
      "id": 42,
      "author_id": 559,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:45.459Z",
      "status": "published",
      "subject_id": 165,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 561,
      "reply_to_id": 42,
      "created_at": "2016-12-08T21:04:45.570Z",
      "status": "published",
      "subject_id": 166,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 563,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:45.703Z",
      "status": "published",
      "subject_id": 167,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 565,
      "reply_to_id": 44,
      "created_at": "2016-12-08T21:04:45.811Z",
      "status": "published",
      "subject_id": 168,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 567,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:45.918Z",
      "status": "reported",
      "subject_id": 169,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 569,
      "reply_to_id": 46,
      "created_at": "2016-12-08T21:04:46.025Z",
      "status": "published",
      "subject_id": 170,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 571,
      "reply_to_id": 46,
      "created_at": "2016-12-08T21:04:46.134Z",
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
	-H "Authorization: Bearer 313a00c0a72e14fbf385bf93c3b75b21efdbc8870b476eb67b5c9035c40f312e"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 2dd659790ce4fe3120065c11fa0424b39d5cea42c23642bde53ee4edf80e0028
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
      "id": 22,
      "author_id": 516,
      "reply_to_id": 21,
      "created_at": "2016-12-08T21:04:43.135Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 520,
      "reply_to_id": 23,
      "created_at": "2016-12-08T21:04:43.351Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 524,
      "reply_to_id": 25,
      "created_at": "2016-12-08T21:04:43.567Z",
      "status": "published",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 526,
      "reply_to_id": 25,
      "created_at": "2016-12-08T21:04:43.676Z",
      "status": "published",
      "subject_id": 150,
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
	-H "Authorization: Bearer 2dd659790ce4fe3120065c11fa0424b39d5cea42c23642bde53ee4edf80e0028"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer c94f0432532179032874a4de08c993390b434b46fe455d266ef02e3985f6d186
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
      "id": 18,
      "author_id": 507,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:04:42.656Z",
      "status": "reported",
      "subject_id": 141,
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
	-H "Authorization: Bearer c94f0432532179032874a4de08c993390b434b46fe455d266ef02e3985f6d186"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/11/republish
Content-Type: application/json
Authorization: Bearer 67b5bcf457ae14d00577b731d5fa5f813a678692275386c7d657e2c27aa59597
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67b5bcf457ae14d00577b731d5fa5f813a678692275386c7d657e2c27aa59597"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/277/chapters
Content-Type: application/json
Authorization: Bearer 251e6f2c534928f9f59aadced64691999f96e5bbb3c14f976f08d24da2397cb7
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
    "id": 153,
    "updated_at": "2016-12-08T21:05:07.635Z",
    "course_id": 277,
    "author_id": 840,
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
curl "api.goskive.com/v2/courses/277/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 251e6f2c534928f9f59aadced64691999f96e5bbb3c14f976f08d24da2397cb7"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer df56cac98fd76f907f45e62a6bac4f6e48452a9e97c773d4359965e3c4645abd
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
    "id": 154,
    "updated_at": "2016-12-08T21:05:07.804Z",
    "course_id": 278,
    "author_id": 842,
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
	-H "Authorization: Bearer df56cac98fd76f907f45e62a6bac4f6e48452a9e97c773d4359965e3c4645abd"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d2cd2b9febaf1f39bd7cf54fcdf5c60805c327b58199bde0c6a12d3001cca150
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
      "id": 171,
      "updated_at": "2016-12-08T21:05:10.170Z",
      "course_id": 289,
      "author_id": 880,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 147",
      "position": 1
    },
    {
      "id": 172,
      "updated_at": "2016-12-08T21:05:10.195Z",
      "course_id": 289,
      "author_id": 881,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 148",
      "position": 2
    },
    {
      "id": 173,
      "updated_at": "2016-12-08T21:05:10.409Z",
      "course_id": 289,
      "author_id": 882,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-08T21:05:10.064Z",
      "questions_updated_at": "2016-12-08T21:05:10.064Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 149",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2cd2b9febaf1f39bd7cf54fcdf5c60805c327b58199bde0c6a12d3001cca150"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2098774184faf1e2c195b93cbce5917af504ea250289082887f97ca2ae6eef25
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
      "updated_at": "2016-12-08T21:05:10.590Z",
      "course_id": 290,
      "author_id": 887,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 150",
      "position": 1
    },
    {
      "id": 175,
      "updated_at": "2016-12-08T21:05:10.616Z",
      "course_id": 290,
      "author_id": 888,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 151",
      "position": 2
    },
    {
      "id": 176,
      "updated_at": "2016-12-08T21:05:10.640Z",
      "course_id": 290,
      "author_id": 889,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 152",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2098774184faf1e2c195b93cbce5917af504ea250289082887f97ca2ae6eef25"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a0043b231fa37cb985349b333af95d36bf88bc2b2b01a73a18010b75e8dfd93c
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
	-H "Authorization: Bearer a0043b231fa37cb985349b333af95d36bf88bc2b2b01a73a18010b75e8dfd93c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/42
Content-Type: application/json
Authorization: Bearer d9122a68f07f8dfcb30b064f82f3a49b1d91d68c87a4f796415f510ea44dd4c9
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/42" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9122a68f07f8dfcb30b064f82f3a49b1d91d68c87a4f796415f510ea44dd4c9"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 440c62e502e80c23645ae9e3ac0b74bfccd6f6e578b8b841e9a8c5d0a18df95d
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
    "creator_id": 120,
    "id": 29,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 30,
    "additional_university_ids": [

    ],
    "discipline_id": 31,
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
    "chapters_updated_at": "2016-12-08T21:04:05.667Z",
    "updated_at": "2016-12-08T21:04:07.023Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 120,
        "chapter_id": 24,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:06.776Z",
        "created_at": "2016-12-08T21:04:06.776Z",
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
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 120,
        "chapter_id": 25,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:06.860Z",
        "created_at": "2016-12-08T21:04:06.860Z",
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
        "author_id": 120,
        "chapter_id": 24,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:06.823Z",
        "created_at": "2016-12-08T21:04:06.823Z",
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
        "author_id": 120,
        "chapter_id": 25,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:06.909Z",
        "created_at": "2016-12-08T21:04:06.909Z",
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
        "author_id": 123,
        "chapter_id": 24,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:06.955Z",
        "created_at": "2016-12-08T21:04:06.955Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 124,
        "chapter_id": 25,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:07.000Z",
        "created_at": "2016-12-08T21:04:07.000Z",
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
        "id": 24,
        "updated_at": "2016-12-08T21:04:06.966Z",
        "course_id": 29,
        "author_id": 120,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T21:04:05.667Z",
        "questions_updated_at": "2016-12-08T21:04:05.667Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 18",
        "position": 1
      },
      {
        "id": 25,
        "updated_at": "2016-12-08T21:04:07.011Z",
        "course_id": 29,
        "author_id": 120,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T21:04:05.667Z",
        "questions_updated_at": "2016-12-08T21:04:05.667Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 19",
        "position": 2
      }
    ],
    "topic_id": 31,
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
	-H "Authorization: Bearer 440c62e502e80c23645ae9e3ac0b74bfccd6f6e578b8b841e9a8c5d0a18df95d"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/43
Content-Type: application/json
Authorization: Bearer 1fbebd4d29715114b66af991bdedaa0666e6f9d6fbb06bc1d2fa200d069ef2c5
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
    "creator_id": 165,
    "id": 43,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 44,
    "additional_university_ids": [

    ],
    "discipline_id": 45,
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
    "updated_at": "2016-12-08T21:04:13.760Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 45,
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
curl "api.goskive.com/v2/courses/43" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fbebd4d29715114b66af991bdedaa0666e6f9d6fbb06bc1d2fa200d069ef2c5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer daf01521907b826564d85d351a8e44c91e10009e8678571805d2a05c437b1795
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
    "creator_id": 170,
    "id": 46,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 47,
    "additional_university_ids": [

    ],
    "discipline_id": 48,
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
    "updated_at": "2016-12-08T21:04:14.224Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 48,
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
	-H "Authorization: Bearer daf01521907b826564d85d351a8e44c91e10009e8678571805d2a05c437b1795"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 86a6f97ccbb6ac4c20c67498d3755361967f7f9e0523a4ee1da943dc01845b2d
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
      "id": 14,
      "user_id": 283,
      "feedbackable_id": 68,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:04:24.714Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 287,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:04:25.025Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 291,
      "feedbackable_id": 70,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:04:25.334Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 295,
      "feedbackable_id": 71,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:04:25.650Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 299,
      "feedbackable_id": 72,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T21:04:25.966Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86a6f97ccbb6ac4c20c67498d3755361967f7f9e0523a4ee1da943dc01845b2d"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 840d370ba3b19cdbe9284b7a38f605f62efe634ca2bca594748d8e8f772a5ea4
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
      "user_id": 320,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T21:04:27.625Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 840d370ba3b19cdbe9284b7a38f605f62efe634ca2bca594748d8e8f772a5ea4"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer a1fdefe94e4fde31b66b0141309a75a002ebb4710fe8b0a0dd4b62b82f37e61c
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
	-H "Authorization: Bearer a1fdefe94e4fde31b66b0141309a75a002ebb4710fe8b0a0dd4b62b82f37e61c"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer 1210317a19451f8bab6b0fb0bd474ec6bef77e09f77d98c9ac9197f5384ff38d
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
    "id": 12,
    "uploader": {
      "id": 368,
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
      "created_at": "2016-12-08T21:04:30.677Z",
      "updated_at": "2016-12-08T21:04:30.677Z"
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
    "created_at": "2016-12-08T21:04:30.782Z",
    "updated_at": "2016-12-08T21:04:30.782Z",
    "course_id": 93,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1210317a19451f8bab6b0fb0bd474ec6bef77e09f77d98c9ac9197f5384ff38d"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/89/feedbacks
Content-Type: application/json
Authorization: Bearer 8ce835f79ad9a440ab3941e23d61d2f45cfe1bc396c50075cf614d8aec884fde
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
      "id": 40,
      "user_id": 945,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:15.095Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 944,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:15.085Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/89/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ce835f79ad9a440ab3941e23d61d2f45cfe1bc396c50075cf614d8aec884fde"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 908ab1d7ceab8f8d3fd2f0ea1be7296ed9c8318429ef0ef706b03ab710378995
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 643,
      "chapter_id": 108,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:50.646Z",
      "created_at": "2016-12-08T21:04:50.646Z",
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 646,
      "chapter_id": 109,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:50.805Z",
      "created_at": "2016-12-08T21:04:50.805Z",
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 649,
      "chapter_id": 110,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:50.963Z",
      "created_at": "2016-12-08T21:04:50.963Z",
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
      "author_id": 652,
      "chapter_id": 111,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:51.121Z",
      "created_at": "2016-12-08T21:04:51.121Z",
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
      "author_id": 655,
      "chapter_id": 112,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:51.283Z",
      "created_at": "2016-12-08T21:04:51.283Z",
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
	-H "Authorization: Bearer 908ab1d7ceab8f8d3fd2f0ea1be7296ed9c8318429ef0ef706b03ab710378995"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer a85e86cb3ae965970301d11fbc0c0089cb78b688b5ce8701a1adbd96983cfd22
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 671,
      "chapter_id": 117,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:52.146Z",
      "created_at": "2016-12-08T21:04:52.146Z",
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
	-H "Authorization: Bearer a85e86cb3ae965970301d11fbc0c0089cb78b688b5ce8701a1adbd96983cfd22"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/republish
Content-Type: application/json
Authorization: Bearer a37bbc5ebef17b0cd564e95f375b6fca2b1cae4c83fbfd39d9ed050b2ab338c9
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a37bbc5ebef17b0cd564e95f375b6fca2b1cae4c83fbfd39d9ed050b2ab338c9"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/128/feedbacks
Content-Type: application/json
Authorization: Bearer d8a5df3b177f6a0a272990fb9194c0ed445a1c4b6db43644d9f9148e7a9b98e6
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
      "user_id": 919,
      "feedbackable_id": 128,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:12.500Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 918,
      "feedbackable_id": 128,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:12.490Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/128/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8a5df3b177f6a0a272990fb9194c0ed445a1c4b6db43644d9f9148e7a9b98e6"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer dcf1dcfafe782a7d8d56a104a95a7fa4a846e43b15f97b4e0a7e4e0f324c0018
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
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 442,
      "chapter_id": 84,
      "position": 84,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:37.498Z",
      "created_at": "2016-12-08T21:04:37.415Z",
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
          "id": 185,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 186,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 445,
      "chapter_id": 85,
      "position": 85,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:37.761Z",
      "created_at": "2016-12-08T21:04:37.678Z",
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
          "id": 187,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 188,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 448,
      "chapter_id": 86,
      "position": 86,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:38.029Z",
      "created_at": "2016-12-08T21:04:37.944Z",
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
    },
    {
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 451,
      "chapter_id": 87,
      "position": 87,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:38.296Z",
      "created_at": "2016-12-08T21:04:38.212Z",
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
          "id": 191,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 192,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 95,
      "obfuscated_id": "uTOhBSQK4CI",
      "author_id": 454,
      "chapter_id": 88,
      "position": 88,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:38.586Z",
      "created_at": "2016-12-08T21:04:38.507Z",
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
          "id": 193,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 194,
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
	-H "Authorization: Bearer dcf1dcfafe782a7d8d56a104a95a7fa4a846e43b15f97b4e0a7e4e0f324c0018"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer d08e04eaf2f2b1d91bc4140bfe8cb4d637ccb683f719c23b815bb1bfb2b96263
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
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 422,
      "chapter_id": 78,
      "position": 78,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:35.769Z",
      "created_at": "2016-12-08T21:04:35.692Z",
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
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d08e04eaf2f2b1d91bc4140bfe8cb4d637ccb683f719c23b815bb1bfb2b96263"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/98/republish
Content-Type: application/json
Authorization: Bearer 235834a6980a268b08e6cd030dc082bba44055edfb85933da7f507abc125eae7
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/98/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 235834a6980a268b08e6cd030dc082bba44055edfb85933da7f507abc125eae7"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2e2d9c08f45450236c10ae5fb19502b6d897b0da45b872b75d7240c5d3d777d9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":261,"published":false}}
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
    "creator_id": 773,
    "id": 254,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 233,
    "additional_university_ids": [

    ],
    "discipline_id": 261,
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
    "updated_at": "2016-12-08T21:05:01.079Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 261,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":261,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e2d9c08f45450236c10ae5fb19502b6d897b0da45b872b75d7240c5d3d777d9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 969187882dc9407d063eaa66f7721391accb1cbee3e6c799828b7f2286333250
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
      "creator_id": 758,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "discipline_id": 248,
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
      "updated_at": "2016-12-08T21:04:59.586Z",
      "shortname": "fu-course-196",
      "topic_id": 248,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 758,
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-197",
      "html_url": "https://goskive.com/course/fu-course-197",
      "slug": "fu-course-197",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "discipline_id": 249,
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
      "updated_at": "2016-12-08T21:04:59.620Z",
      "shortname": "fu-course-197",
      "topic_id": 249,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 197",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 759,
      "id": 243,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-198",
      "html_url": "https://goskive.com/course/fu-course-198",
      "slug": "fu-course-198",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "discipline_id": 250,
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
      "updated_at": "2016-12-08T21:04:59.661Z",
      "shortname": "fu-course-198",
      "topic_id": 250,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 198",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 759,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "discipline_id": 251,
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
      "chapters_updated_at": "2016-12-08T21:04:59.505Z",
      "updated_at": "2016-12-08T21:04:59.941Z",
      "shortname": "fu-course-199",
      "topic_id": 251,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 969187882dc9407d063eaa66f7721391accb1cbee3e6c799828b7f2286333250"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 12fca700f545b03ac0316be3fc94512324f86ab2765b989a038f64d49c484bff
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
      "creator_id": 764,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-200",
      "html_url": "https://goskive.com/course/fu-course-200",
      "slug": "fu-course-200",
      "university_id": 228,
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
      "updated_at": "2016-12-08T21:05:00.129Z",
      "shortname": "fu-course-200",
      "topic_id": 252,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 200",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 764,
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-201",
      "html_url": "https://goskive.com/course/fu-course-201",
      "slug": "fu-course-201",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 253,
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
      "updated_at": "2016-12-08T21:05:00.163Z",
      "shortname": "fu-course-201",
      "topic_id": 253,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 201",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 765,
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-202",
      "html_url": "https://goskive.com/course/fu-course-202",
      "slug": "fu-course-202",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 254,
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
      "updated_at": "2016-12-08T21:05:00.205Z",
      "shortname": "fu-course-202",
      "topic_id": 254,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 202",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 765,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 255,
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
      "updated_at": "2016-12-08T21:05:00.239Z",
      "shortname": "fu-course-203",
      "topic_id": 255,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12fca700f545b03ac0316be3fc94512324f86ab2765b989a038f64d49c484bff"
```
