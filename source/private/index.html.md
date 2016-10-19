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
DELETE /v2/chapters/13
Content-Type: application/json
Authorization: Bearer ba0ad37ca4d22092c36f090f88a283f7c9e8aa580faeffc5f8ca307984dfa940
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba0ad37ca4d22092c36f090f88a283f7c9e8aa580faeffc5f8ca307984dfa940"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/10
Content-Type: application/json
Authorization: Bearer c18a0eda77821f54a1ab9ffcb9299d63f8749d1afaf706c150cd641547025f15
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
    "updated_at": "2016-10-19T08:04:11.473Z",
    "course_id": 14,
    "author_id": 43,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-19T08:04:10.931Z",
    "questions_updated_at": "2016-10-19T08:04:10.931Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 46,
        "chapter_id": 10,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:11.416Z",
        "created_at": "2016-10-19T08:04:11.416Z",
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
        "author_id": 47,
        "chapter_id": 10,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:11.455Z",
        "created_at": "2016-10-19T08:04:11.455Z",
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
        "author_id": 44,
        "chapter_id": 10,
        "position": 7,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:11.146Z",
        "created_at": "2016-10-19T08:04:11.036Z",
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
        "author_id": 45,
        "chapter_id": 10,
        "position": 8,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:11.336Z",
        "created_at": "2016-10-19T08:04:11.216Z",
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
	-H "Authorization: Bearer c18a0eda77821f54a1ab9ffcb9299d63f8749d1afaf706c150cd641547025f15"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/8
Content-Type: application/json
Authorization: Bearer ac7e982cb43e7ec1b860f994dbf0b9aa5e61df8da5881a87f356437589adf342
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
    "updated_at": "2016-10-19T08:04:10.736Z",
    "course_id": 12,
    "author_id": 38,
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
	-H "Authorization: Bearer ac7e982cb43e7ec1b860f994dbf0b9aa5e61df8da5881a87f356437589adf342"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer f18a545c30aa860e413ef65fa554ad0d692494028dce59eb174fac1081cbee60
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
	-H "Authorization: Bearer f18a545c30aa860e413ef65fa554ad0d692494028dce59eb174fac1081cbee60"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 58f3a9fac1fc705f848c531f1a67d98395fec86d89dfc0def6d6bd688ab7d149
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
      "author_id": 885,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:18.723Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 887,
      "reply_to_id": 27,
      "created_at": "2016-10-19T08:05:18.800Z",
      "status": "published",
      "subject_id": 277,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 889,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:18.880Z",
      "status": "published",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 891,
      "reply_to_id": 29,
      "created_at": "2016-10-19T08:05:18.957Z",
      "status": "published",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 893,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:19.037Z",
      "status": "reported",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 895,
      "reply_to_id": 31,
      "created_at": "2016-10-19T08:05:19.117Z",
      "status": "published",
      "subject_id": 281,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 897,
      "reply_to_id": 31,
      "created_at": "2016-10-19T08:05:19.198Z",
      "status": "published",
      "subject_id": 282,
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
	-H "Authorization: Bearer 58f3a9fac1fc705f848c531f1a67d98395fec86d89dfc0def6d6bd688ab7d149"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer f41f559bb2e16718dc33796da8c7d36974aa956aa857d952b027c2cf4a40999c
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
      "author_id": 900,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:19.334Z",
      "status": "published",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 902,
      "reply_to_id": 34,
      "created_at": "2016-10-19T08:05:19.415Z",
      "status": "published",
      "subject_id": 284,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 904,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:19.497Z",
      "status": "published",
      "subject_id": 285,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 906,
      "reply_to_id": 36,
      "created_at": "2016-10-19T08:05:19.576Z",
      "status": "published",
      "subject_id": 286,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 908,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:19.655Z",
      "status": "reported",
      "subject_id": 287,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 910,
      "reply_to_id": 38,
      "created_at": "2016-10-19T08:05:19.731Z",
      "status": "published",
      "subject_id": 288,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 912,
      "reply_to_id": 38,
      "created_at": "2016-10-19T08:05:19.809Z",
      "status": "published",
      "subject_id": 289,
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
	-H "Authorization: Bearer f41f559bb2e16718dc33796da8c7d36974aa956aa857d952b027c2cf4a40999c"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer fead91220191619e9efd23114c85888857890b0a3fabe7260601c29cd5ada240
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
      "id": 49,
      "author_id": 932,
      "reply_to_id": 48,
      "created_at": "2016-10-19T08:05:20.666Z",
      "status": "published",
      "subject_id": 298,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 936,
      "reply_to_id": 50,
      "created_at": "2016-10-19T08:05:20.820Z",
      "status": "published",
      "subject_id": 300,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 940,
      "reply_to_id": 52,
      "created_at": "2016-10-19T08:05:20.974Z",
      "status": "published",
      "subject_id": 302,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 54,
      "author_id": 942,
      "reply_to_id": 52,
      "created_at": "2016-10-19T08:05:21.052Z",
      "status": "published",
      "subject_id": 303,
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
	-H "Authorization: Bearer fead91220191619e9efd23114c85888857890b0a3fabe7260601c29cd5ada240"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer c8c165688a7f887d2fdbc26d0ea4a254dae4d6016740680c169d657d5d93ac1b
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
      "id": 24,
      "author_id": 878,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:05:18.421Z",
      "status": "reported",
      "subject_id": 273,
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
	-H "Authorization: Bearer c8c165688a7f887d2fdbc26d0ea4a254dae4d6016740680c169d657d5d93ac1b"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/58/republish
Content-Type: application/json
Authorization: Bearer 8c3b9b1ad7b40d110c0695fd4410d9152ab1151acc8c3ce6d8f354fe9cf888be
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/58/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c3b9b1ad7b40d110c0695fd4410d9152ab1151acc8c3ce6d8f354fe9cf888be"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/99/chapters
Content-Type: application/json
Authorization: Bearer f61f7a665fcdd2441e45fd8175f5f49f6cbedfe3b4a58ea25e5cd897b0090302
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
    "id": 92,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T08:04:42.289Z",
    "course_id": 99,
    "author_id": 408,
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
curl "api.goskive.com/v2/courses/99/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f61f7a665fcdd2441e45fd8175f5f49f6cbedfe3b4a58ea25e5cd897b0090302"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3df28da22a65ef968da12b0a22b0b0c8614922e934904b55f3895d3349056f2e
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
    "id": 93,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T08:04:42.511Z",
    "course_id": 101,
    "author_id": 412,
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
	-H "Authorization: Bearer 3df28da22a65ef968da12b0a22b0b0c8614922e934904b55f3895d3349056f2e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c9ceea7112cced48a6e54c738018b8d50e9dfe70abc80b2b5e04fb6281af7205
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
      "id": 71,
      "title": "Clever Chapter Title 56",
      "position": 1,
      "updated_at": "2016-10-19T08:04:39.997Z",
      "course_id": 88,
      "author_id": 362,
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
      "id": 72,
      "title": "Clever Chapter Title 57",
      "position": 2,
      "updated_at": "2016-10-19T08:04:40.025Z",
      "course_id": 88,
      "author_id": 363,
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
      "id": 73,
      "title": "Clever Chapter Title 58",
      "position": 3,
      "updated_at": "2016-10-19T08:04:40.260Z",
      "course_id": 88,
      "author_id": 364,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-19T08:04:39.918Z",
      "questions_updated_at": "2016-10-19T08:04:39.918Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9ceea7112cced48a6e54c738018b8d50e9dfe70abc80b2b5e04fb6281af7205"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 873a936d6156680ba9756418d85bf0160bca362aefe275f9901b61f7d69a1fa6
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
      "id": 74,
      "title": "Clever Chapter Title 59",
      "position": 1,
      "updated_at": "2016-10-19T08:04:40.425Z",
      "course_id": 89,
      "author_id": 369,
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
      "id": 75,
      "title": "Clever Chapter Title 60",
      "position": 2,
      "updated_at": "2016-10-19T08:04:40.447Z",
      "course_id": 89,
      "author_id": 370,
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
      "id": 76,
      "title": "Clever Chapter Title 61",
      "position": 3,
      "updated_at": "2016-10-19T08:04:40.470Z",
      "course_id": 89,
      "author_id": 371,
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
	-H "Authorization: Bearer 873a936d6156680ba9756418d85bf0160bca362aefe275f9901b61f7d69a1fa6"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer adf3d1d16cc12c63978e5787abc4062e4b1359d1e2c1b3cd8c6ceb853797c46e
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
	-H "Authorization: Bearer adf3d1d16cc12c63978e5787abc4062e4b1359d1e2c1b3cd8c6ceb853797c46e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/135
Content-Type: application/json
Authorization: Bearer 51954e4d254790e13e8403b2ff0cbae5abbb687f18214d0c0960fd35b1546d71
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/135" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51954e4d254790e13e8403b2ff0cbae5abbb687f18214d0c0960fd35b1546d71"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer c92cbfec799ceab4c116dd13bf77131ccbfcf610d175ab0b2a7cb0e07d2232a0
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
    "creator_id": 534,
    "id": 139,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 146,
    "additional_university_ids": [

    ],
    "topic_id": 151,
    "discipline_id": 152,
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
    "chapters_updated_at": "2016-10-19T08:04:52.894Z",
    "updated_at": "2016-10-19T08:04:54.212Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 122,
        "title": "Clever Chapter Title 104",
        "position": 1,
        "updated_at": "2016-10-19T08:04:54.170Z",
        "course_id": 139,
        "author_id": 534,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T08:04:52.894Z",
        "questions_updated_at": "2016-10-19T08:04:52.894Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 123,
        "title": "Clever Chapter Title 105",
        "position": 2,
        "updated_at": "2016-10-19T08:04:54.206Z",
        "course_id": 139,
        "author_id": 534,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T08:04:52.894Z",
        "questions_updated_at": "2016-10-19T08:04:52.894Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 534,
        "chapter_id": 122,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.027Z",
        "created_at": "2016-10-19T08:04:54.027Z",
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
        "author_id": 534,
        "chapter_id": 123,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.091Z",
        "created_at": "2016-10-19T08:04:54.091Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 534,
        "chapter_id": 122,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.063Z",
        "created_at": "2016-10-19T08:04:54.063Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 534,
        "chapter_id": 123,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.126Z",
        "created_at": "2016-10-19T08:04:54.126Z",
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
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 537,
        "chapter_id": 122,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.162Z",
        "created_at": "2016-10-19T08:04:54.162Z",
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
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 538,
        "chapter_id": 123,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:54.197Z",
        "created_at": "2016-10-19T08:04:54.197Z",
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
	-H "Authorization: Bearer c92cbfec799ceab4c116dd13bf77131ccbfcf610d175ab0b2a7cb0e07d2232a0"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/144
Content-Type: application/json
Authorization: Bearer 8d5345d08e550be013dee5023ba8466e105670545c3ae8ee578eb78b30f2fb4b
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
    "creator_id": 547,
    "id": 144,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 151,
    "additional_university_ids": [

    ],
    "topic_id": 156,
    "discipline_id": 157,
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
    "updated_at": "2016-10-19T08:04:54.850Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/144" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d5345d08e550be013dee5023ba8466e105670545c3ae8ee578eb78b30f2fb4b"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b0bc8018f7d974ac267b0ff66030cef808dc9e18fe29ace372fd6dd1ad0bdadb
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
    "creator_id": 543,
    "id": 142,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 149,
    "additional_university_ids": [

    ],
    "topic_id": 154,
    "discipline_id": 155,
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
    "updated_at": "2016-10-19T08:04:54.631Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0bc8018f7d974ac267b0ff66030cef808dc9e18fe29ace372fd6dd1ad0bdadb"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer c8ab8654727098bf51e9a89ff4c1ec6332a853c4a3205a0c679b54a7198c6a8b
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
      "id": 22,
      "user_id": 202,
      "feedbackable_id": 33,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:22.930Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 206,
      "feedbackable_id": 34,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:23.261Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 210,
      "feedbackable_id": 35,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:23.583Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 214,
      "feedbackable_id": 36,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:23.894Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 218,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T08:04:24.211Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8ab8654727098bf51e9a89ff4c1ec6332a853c4a3205a0c679b54a7198c6a8b"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer b865e590c55febae2db9d663887564ba06ef315adaa590d750ac0452d3ec5101
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
      "id": 21,
      "user_id": 197,
      "feedbackable_id": 32,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T08:04:22.561Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b865e590c55febae2db9d663887564ba06ef315adaa590d750ac0452d3ec5101"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer 286efd142a18be43bb1bd8352049e212bc32c3502498aed8f3d34cd106b7a22d
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Authorization: Bearer 286efd142a18be43bb1bd8352049e212bc32c3502498aed8f3d34cd106b7a22d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer a096892d98158458df55d6016812ca4c07e1eac9adf29b82dbff21daaed25897
Content-Type: application/json
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
    "id": 7,
    "uploader": {
      "id": 662,
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
      "created_at": "2016-10-19T08:05:00.339Z",
      "updated_at": "2016-10-19T08:05:00.339Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-19T08:05:00.406Z",
    "updated_at": "2016-10-19T08:05:00.406Z",
    "course_id": 182,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Authorization: Bearer a096892d98158458df55d6016812ca4c07e1eac9adf29b82dbff21daaed25897" \
	-H "Content-Type: application/json"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/28/feedbacks
Content-Type: application/json
Authorization: Bearer 7adf22c9cdbc0833377e20740955281f16ddf8ff6ca9e7bd550a880e17312684
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
      "user_id": 453,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:44.625Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 452,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:44.615Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/28/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7adf22c9cdbc0833377e20740955281f16ddf8ff6ca9e7bd550a880e17312684"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 08d4379781cab0e6f8481b08dff12cac82803079cab08809206c39170ae258d4
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
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 604,
      "chapter_id": 136,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:57.728Z",
      "created_at": "2016-10-19T08:04:57.728Z",
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
      "author_id": 607,
      "chapter_id": 137,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:57.850Z",
      "created_at": "2016-10-19T08:04:57.850Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 610,
      "chapter_id": 138,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:57.974Z",
      "created_at": "2016-10-19T08:04:57.974Z",
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 613,
      "chapter_id": 139,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:58.097Z",
      "created_at": "2016-10-19T08:04:58.097Z",
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
      "author_id": 616,
      "chapter_id": 140,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:58.221Z",
      "created_at": "2016-10-19T08:04:58.221Z",
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
	-H "Authorization: Bearer 08d4379781cab0e6f8481b08dff12cac82803079cab08809206c39170ae258d4"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer afb8344f8349a675f116c0c3309af13a56cb2818008c57bc7169ab67e83940e2
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
      "author_id": 632,
      "chapter_id": 145,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:58.911Z",
      "created_at": "2016-10-19T08:04:58.911Z",
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
	-H "Authorization: Bearer afb8344f8349a675f116c0c3309af13a56cb2818008c57bc7169ab67e83940e2"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/68/republish
Content-Type: application/json
Authorization: Bearer b14c58429fb7f2c2ed84352c42c4838b12a0be78c3214fa99c739d0599e8adca
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
	-H "Authorization: Bearer b14c58429fb7f2c2ed84352c42c4838b12a0be78c3214fa99c739d0599e8adca"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/131/feedbacks
Content-Type: application/json
Authorization: Bearer 9fb807afee68a5eff8b25634f1deab80b31ce3ab5ba9e4b6305aad540ebe6b5a
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
      "user_id": 856,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:05:17.081Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 855,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:05:17.070Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/131/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9fb807afee68a5eff8b25634f1deab80b31ce3ab5ba9e4b6305aad540ebe6b5a"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer c2d535b14fe11c65b986adb5fdf0613f27cc61e84dd132419523a81820164057
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
      "id": 106,
      "obfuscated_id": "GEL902caNek",
      "author_id": 751,
      "chapter_id": 167,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:07.593Z",
      "created_at": "2016-10-19T08:05:07.486Z",
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
          "id": 214,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 215,
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
      "author_id": 742,
      "chapter_id": 164,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:06.823Z",
      "created_at": "2016-10-19T08:05:06.716Z",
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
          "id": 208,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 209,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 104,
      "obfuscated_id": "nIg2bhYRjos",
      "author_id": 745,
      "chapter_id": 165,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:07.081Z",
      "created_at": "2016-10-19T08:05:06.973Z",
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
          "id": 210,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 211,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 105,
      "obfuscated_id": "3yX9LpVrF_M",
      "author_id": 748,
      "chapter_id": 166,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:07.338Z",
      "created_at": "2016-10-19T08:05:07.231Z",
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
          "id": 212,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 213,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 107,
      "obfuscated_id": "_2rgp7tgq8o",
      "author_id": 754,
      "chapter_id": 168,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:07.842Z",
      "created_at": "2016-10-19T08:05:07.741Z",
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
          "id": 216,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 217,
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
	-H "Authorization: Bearer c2d535b14fe11c65b986adb5fdf0613f27cc61e84dd132419523a81820164057"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer f6014b7f9e43d4ef4750f985308245c6aa1ad7191fc53206e8a820961d24e1a8
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
      "id": 102,
      "obfuscated_id": "jFy90P7ldB4",
      "author_id": 738,
      "chapter_id": 163,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:05:06.503Z",
      "created_at": "2016-10-19T08:05:06.402Z",
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
          "id": 206,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 207,
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
	-H "Authorization: Bearer f6014b7f9e43d4ef4750f985308245c6aa1ad7191fc53206e8a820961d24e1a8"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/117/republish
Content-Type: application/json
Authorization: Bearer 0b15410521363f95dedd101d7fce0e0a0c3a681ea4727dda01647e0f6c52d4b3
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/117/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b15410521363f95dedd101d7fce0e0a0c3a681ea4727dda01647e0f6c52d4b3"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 32ed1874ab97b5fcbb57ea69beab26c32c53106959da18f464151f5bd6e64556
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":238,"published":false}}
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
    "creator_id": 722,
    "id": 226,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 211,
    "additional_university_ids": [

    ],
    "topic_id": 238,
    "discipline_id": 239,
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
    "updated_at": "2016-10-19T08:05:05.084Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":238,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32ed1874ab97b5fcbb57ea69beab26c32c53106959da18f464151f5bd6e64556"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ddc7847957469412fec2d61f306b3e706cf03e87b6ed05116dddb5ea71fad7c4
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
      "creator_id": 690,
      "id": 200,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 212,
      "discipline_id": 213,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "updated_at": "2016-10-19T08:05:02.350Z",
      "shortname": "fu-course-132"
    },
    {
      "creator_id": 690,
      "id": 201,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-133",
      "html_url": "https://goskive.com/course/fu-course-133",
      "slug": "fu-course-133",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 213,
      "discipline_id": 214,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 133",
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
      "updated_at": "2016-10-19T08:05:02.387Z",
      "shortname": "fu-course-133"
    },
    {
      "creator_id": 691,
      "id": 202,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 214,
      "discipline_id": 215,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
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
      "updated_at": "2016-10-19T08:05:02.430Z",
      "shortname": "fu-course-134"
    },
    {
      "creator_id": 691,
      "id": 203,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 215,
      "discipline_id": 216,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "chapters_updated_at": "2016-10-19T08:05:02.693Z",
      "updated_at": "2016-10-19T08:05:02.699Z",
      "shortname": "fu-course-135"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddc7847957469412fec2d61f306b3e706cf03e87b6ed05116dddb5ea71fad7c4"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 187e165f401c6c81d73a15c513488ab975ca51ab0926c9d9745000f5ad8e4679
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
      "creator_id": 697,
      "id": 204,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 216,
      "discipline_id": 217,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
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
      "updated_at": "2016-10-19T08:05:02.888Z",
      "shortname": "fu-course-136"
    },
    {
      "creator_id": 697,
      "id": 205,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 217,
      "discipline_id": 218,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
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
      "updated_at": "2016-10-19T08:05:02.924Z",
      "shortname": "fu-course-137"
    },
    {
      "creator_id": 698,
      "id": 206,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 218,
      "discipline_id": 219,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
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
      "updated_at": "2016-10-19T08:05:02.968Z",
      "shortname": "fu-course-138"
    },
    {
      "creator_id": 698,
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 219,
      "discipline_id": 220,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
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
      "updated_at": "2016-10-19T08:05:03.029Z",
      "shortname": "fu-course-139"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 187e165f401c6c81d73a15c513488ab975ca51ab0926c9d9745000f5ad8e4679"
```
