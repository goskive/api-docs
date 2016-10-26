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
DELETE /v2/chapters/16
Content-Type: application/json
Authorization: Bearer 9573cee2471d6875247051f66800ef070b07e1b9a02a7d6977f95493ccfd960f
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9573cee2471d6875247051f66800ef070b07e1b9a02a7d6977f95493ccfd960f"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/15
Content-Type: application/json
Authorization: Bearer 1710f834efa6566df5727ba448edf9da08143db83cc398a8403ae2f63b9f2d23
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
    "id": 15,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T10:35:16.499Z",
    "course_id": 93,
    "author_id": 185,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-26T10:35:15.995Z",
    "questions_updated_at": "2016-10-26T10:35:15.995Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 188,
        "chapter_id": 15,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:16.448Z",
        "created_at": "2016-10-26T10:35:16.448Z",
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
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 189,
        "chapter_id": 15,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:16.482Z",
        "created_at": "2016-10-26T10:35:16.482Z",
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
        "author_id": 186,
        "chapter_id": 15,
        "position": 7,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:16.199Z",
        "created_at": "2016-10-26T10:35:16.092Z",
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
        "author_id": 187,
        "chapter_id": 15,
        "position": 8,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:16.383Z",
        "created_at": "2016-10-26T10:35:16.266Z",
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
curl "api.goskive.com/v2/chapters/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1710f834efa6566df5727ba448edf9da08143db83cc398a8403ae2f63b9f2d23"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/20
Content-Type: application/json
Authorization: Bearer a7469553c98e33d064dad5bed3b202b0388cd182b30bdef53d1cf7527a04c744
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
    "id": 20,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T10:35:17.606Z",
    "course_id": 98,
    "author_id": 204,
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
curl "api.goskive.com/v2/chapters/20" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7469553c98e33d064dad5bed3b202b0388cd182b30bdef53d1cf7527a04c744"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 6c7eeb961629050c1e7fa1266f6c2c7a129419d1a0ff63095c02dbc08009a85c
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c7eeb961629050c1e7fa1266f6c2c7a129419d1a0ff63095c02dbc08009a85c"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 1c90441b71c8e43172ad2c6fe7b8f20d4893607adf8cebe357b206f156fd1499
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
      "author_id": 143,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:13.911Z",
      "status": "published",
      "subject_id": 78,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 145,
      "reply_to_id": 28,
      "created_at": "2016-10-26T10:35:13.989Z",
      "status": "published",
      "subject_id": 79,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 147,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:14.071Z",
      "status": "published",
      "subject_id": 80,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 149,
      "reply_to_id": 30,
      "created_at": "2016-10-26T10:35:14.149Z",
      "status": "published",
      "subject_id": 81,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 151,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:14.227Z",
      "status": "reported",
      "subject_id": 82,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 153,
      "reply_to_id": 32,
      "created_at": "2016-10-26T10:35:14.308Z",
      "status": "published",
      "subject_id": 83,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 155,
      "reply_to_id": 32,
      "created_at": "2016-10-26T10:35:14.388Z",
      "status": "published",
      "subject_id": 84,
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
	-H "Authorization: Bearer 1c90441b71c8e43172ad2c6fe7b8f20d4893607adf8cebe357b206f156fd1499"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 8e25b5f0380c0777b19105fb83b29928dc73957ae4c1830ab8fd4e6d04091175
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
      "author_id": 158,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:14.522Z",
      "status": "published",
      "subject_id": 85,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 160,
      "reply_to_id": 35,
      "created_at": "2016-10-26T10:35:14.600Z",
      "status": "published",
      "subject_id": 86,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 162,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:14.680Z",
      "status": "published",
      "subject_id": 87,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 164,
      "reply_to_id": 37,
      "created_at": "2016-10-26T10:35:14.761Z",
      "status": "published",
      "subject_id": 88,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 166,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:14.841Z",
      "status": "reported",
      "subject_id": 89,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 168,
      "reply_to_id": 39,
      "created_at": "2016-10-26T10:35:14.920Z",
      "status": "published",
      "subject_id": 90,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 170,
      "reply_to_id": 39,
      "created_at": "2016-10-26T10:35:15.001Z",
      "status": "published",
      "subject_id": 91,
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
	-H "Authorization: Bearer 8e25b5f0380c0777b19105fb83b29928dc73957ae4c1830ab8fd4e6d04091175"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer df490472e6f3648a1c6883abb6782986c5a6ca9155e83c7be1528b228f35e373
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
      "id": 8,
      "author_id": 100,
      "reply_to_id": 7,
      "created_at": "2016-10-26T10:35:12.176Z",
      "status": "published",
      "subject_id": 58,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 104,
      "reply_to_id": 9,
      "created_at": "2016-10-26T10:35:12.334Z",
      "status": "published",
      "subject_id": 60,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 108,
      "reply_to_id": 11,
      "created_at": "2016-10-26T10:35:12.491Z",
      "status": "published",
      "subject_id": 62,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 110,
      "reply_to_id": 11,
      "created_at": "2016-10-26T10:35:12.570Z",
      "status": "published",
      "subject_id": 63,
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
	-H "Authorization: Bearer df490472e6f3648a1c6883abb6782986c5a6ca9155e83c7be1528b228f35e373"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 54ca5d3334db346be9b322bcc9d62b6341663733ee43eb74bce4dfea0209a295
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
      "author_id": 121,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:13.022Z",
      "status": "reported",
      "subject_id": 68,
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
	-H "Authorization: Bearer 54ca5d3334db346be9b322bcc9d62b6341663733ee43eb74bce4dfea0209a295"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer 28ba65f75187a0b5dabbc4a3a6c999276d57db4ef85689eafd8fb657ba22205e
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
	-H "Authorization: Bearer 28ba65f75187a0b5dabbc4a3a6c999276d57db4ef85689eafd8fb657ba22205e"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/269/chapters
Content-Type: application/json
Authorization: Bearer cce8c1f703668bd86d203a35b83d01287ce1125a07b362e3d49905b209047c53
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
    "id": 169,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T10:36:06.305Z",
    "course_id": 269,
    "author_id": 824,
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
curl "api.goskive.com/v2/courses/269/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cce8c1f703668bd86d203a35b83d01287ce1125a07b362e3d49905b209047c53"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 76cee26b39a56032de6e35732ae57ee98f73e373f587c3efdf61b0912717978f
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
    "updated_at": "2016-10-26T10:36:06.701Z",
    "course_id": 272,
    "author_id": 830,
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
	-H "Authorization: Bearer 76cee26b39a56032de6e35732ae57ee98f73e373f587c3efdf61b0912717978f"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3e9f49e871fe35009a1e3c80b9375cf9e78357990c0992584e05c526d5630255
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
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-26T10:36:05.587Z",
      "course_id": 266,
      "author_id": 810,
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
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-26T10:36:05.609Z",
      "course_id": 266,
      "author_id": 811,
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
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-26T10:36:05.852Z",
      "course_id": 266,
      "author_id": 812,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-26T10:36:05.514Z",
      "questions_updated_at": "2016-10-26T10:36:05.514Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e9f49e871fe35009a1e3c80b9375cf9e78357990c0992584e05c526d5630255"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b8b8eb39736920b93ccfc5b3de3db3b96afc2740e144db2ece7af28e9642576d
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-26T10:36:06.092Z",
      "course_id": 268,
      "author_id": 819,
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
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-26T10:36:06.115Z",
      "course_id": 268,
      "author_id": 820,
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
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-26T10:36:06.139Z",
      "course_id": 268,
      "author_id": 821,
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
	-H "Authorization: Bearer b8b8eb39736920b93ccfc5b3de3db3b96afc2740e144db2ece7af28e9642576d"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e61f365fd3cc3e8863cf3171a831ce27b48c5a68b573b3e55e9d3446749cbc61
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
	-H "Authorization: Bearer e61f365fd3cc3e8863cf3171a831ce27b48c5a68b573b3e55e9d3446749cbc61"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/175
Content-Type: application/json
Authorization: Bearer 1ae19e27fc7bd248b582711087dcb781944cf790e15d461c1e6185f5524d4317
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/175" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ae19e27fc7bd248b582711087dcb781944cf790e15d461c1e6185f5524d4317"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 359d1d025fbded3f3b4852a009e269e702d8b5df8128bd5817a9ceb7a29d583d
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
    "creator_id": 449,
    "id": 177,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 157,
    "additional_university_ids": [

    ],
    "topic_id": 186,
    "discipline_id": 187,
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
    "chapters_updated_at": "2016-10-26T10:35:36.272Z",
    "updated_at": "2016-10-26T10:35:37.649Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 65,
        "title": "Clever Chapter Title 50",
        "position": 1,
        "updated_at": "2016-10-26T10:35:37.604Z",
        "course_id": 177,
        "author_id": 449,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T10:35:36.272Z",
        "questions_updated_at": "2016-10-26T10:35:36.272Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 66,
        "title": "Clever Chapter Title 51",
        "position": 2,
        "updated_at": "2016-10-26T10:35:37.641Z",
        "course_id": 177,
        "author_id": 449,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T10:35:36.272Z",
        "questions_updated_at": "2016-10-26T10:35:36.272Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 449,
        "chapter_id": 65,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.445Z",
        "created_at": "2016-10-26T10:35:37.445Z",
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
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 449,
        "chapter_id": 66,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.517Z",
        "created_at": "2016-10-26T10:35:37.517Z",
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
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 449,
        "chapter_id": 65,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.484Z",
        "created_at": "2016-10-26T10:35:37.484Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 449,
        "chapter_id": 66,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.556Z",
        "created_at": "2016-10-26T10:35:37.556Z",
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
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 452,
        "chapter_id": 65,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.595Z",
        "created_at": "2016-10-26T10:35:37.595Z",
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
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 453,
        "chapter_id": 66,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.632Z",
        "created_at": "2016-10-26T10:35:37.632Z",
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
	-H "Authorization: Bearer 359d1d025fbded3f3b4852a009e269e702d8b5df8128bd5817a9ceb7a29d583d"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/161
Content-Type: application/json
Authorization: Bearer 048976df61f3c029eaed80a659211c57f536588c10dde0d31574ef151b495197
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
    "creator_id": 412,
    "id": 161,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 141,
    "additional_university_ids": [

    ],
    "topic_id": 170,
    "discipline_id": 171,
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
    "updated_at": "2016-10-26T10:35:32.652Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/161" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 048976df61f3c029eaed80a659211c57f536588c10dde0d31574ef151b495197"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 725e007baa288d43f07294aa89de99352e284ca6e8d8e36f9ddc7200ba00dacf
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
    "creator_id": 414,
    "id": 162,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 142,
    "additional_university_ids": [

    ],
    "topic_id": 171,
    "discipline_id": 172,
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
    "updated_at": "2016-10-26T10:35:32.784Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 725e007baa288d43f07294aa89de99352e284ca6e8d8e36f9ddc7200ba00dacf"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 38bdc91ae5423c709e33c3c664130ac0a982a32fa489d9da65f0e59ea11731b5
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
      "user_id": 650,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:55.740Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 654,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:56.024Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 658,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:56.315Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 662,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:56.602Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 666,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T10:35:56.894Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38bdc91ae5423c709e33c3c664130ac0a982a32fa489d9da65f0e59ea11731b5"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 8648cb8af37290a50ef9c1c388ddb692dbff716ace08481be5d72a8c01d0abe7
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
      "id": 12,
      "user_id": 608,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T10:35:52.783Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8648cb8af37290a50ef9c1c388ddb692dbff716ace08481be5d72a8c01d0abe7"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer dc0b284c661cf8992a5e5850129ed89eed5b04ed9b4f4a92d12d5cf8d133dada
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
	-H "Authorization: Bearer dc0b284c661cf8992a5e5850129ed89eed5b04ed9b4f4a92d12d5cf8d133dada"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/6/metadata
Content-Type: application/json
Authorization: Bearer 3ea1db7ea041796d81c31151e4f9d2adb403acb3a1ad6a2ade2355cec4456106
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
    "id": 6,
    "uploader": {
      "id": 890,
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
      "created_at": "2016-10-26T10:36:12.854Z",
      "updated_at": "2016-10-26T10:36:12.854Z"
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
    "created_at": "2016-10-26T10:36:12.928Z",
    "updated_at": "2016-10-26T10:36:12.928Z",
    "course_id": 289,
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
curl "api.goskive.com/v2/files/6/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ea1db7ea041796d81c31151e4f9d2adb403acb3a1ad6a2ade2355cec4456106"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/77/feedbacks
Content-Type: application/json
Authorization: Bearer 041b3512912a5b53885d2f0893a1cdc55d7a4257c72fa25f873ccc7283025887
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
      "id": 39,
      "user_id": 727,
      "feedbackable_id": 77,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:00.905Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 38,
      "user_id": 726,
      "feedbackable_id": 77,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:00.894Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/77/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 041b3512912a5b53885d2f0893a1cdc55d7a4257c72fa25f873ccc7283025887"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 3e6daa56c25f9f6c9fb6974273e656552446f5592af2c623515867fd35642817
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 307,
      "chapter_id": 39,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:26.128Z",
      "created_at": "2016-10-26T10:35:26.128Z",
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
      "author_id": 310,
      "chapter_id": 40,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:26.273Z",
      "created_at": "2016-10-26T10:35:26.273Z",
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
      "author_id": 313,
      "chapter_id": 41,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:26.423Z",
      "created_at": "2016-10-26T10:35:26.423Z",
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 316,
      "chapter_id": 42,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:26.578Z",
      "created_at": "2016-10-26T10:35:26.578Z",
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 319,
      "chapter_id": 43,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:26.738Z",
      "created_at": "2016-10-26T10:35:26.738Z",
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
	-H "Authorization: Bearer 3e6daa56c25f9f6c9fb6974273e656552446f5592af2c623515867fd35642817"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer a258f8391f730f369805b6b0a84b5b845f5371af6f22f9b8ef60f37d2f453af4
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 303,
      "chapter_id": 38,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:25.949Z",
      "created_at": "2016-10-26T10:35:25.949Z",
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
	-H "Authorization: Bearer a258f8391f730f369805b6b0a84b5b845f5371af6f22f9b8ef60f37d2f453af4"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/16/republish
Content-Type: application/json
Authorization: Bearer 56a651fa425bc7dc5d7e5b1689009082e55ffca228a283527db2e33655f994af
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56a651fa425bc7dc5d7e5b1689009082e55ffca228a283527db2e33655f994af"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/100/feedbacks
Content-Type: application/json
Authorization: Bearer bd99ec0cf4a6fbc14a2551a29b7ccf0e069fa23baea99f99aad88939608c4f55
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
      "id": 37,
      "user_id": 716,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:00.270Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 715,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:00.260Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/100/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd99ec0cf4a6fbc14a2551a29b7ccf0e069fa23baea99f99aad88939608c4f55"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer b1910a2465a82ebdcbe41c10c9f75bd4e8272a8b4cb02eeef570bd800d5237a9
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 518,
      "chapter_id": 87,
      "position": 61,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:45.541Z",
      "created_at": "2016-10-26T10:35:45.425Z",
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
          "id": 127,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 128,
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
      "author_id": 509,
      "chapter_id": 84,
      "position": 58,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:44.730Z",
      "created_at": "2016-10-26T10:35:44.619Z",
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
          "id": 121,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 122,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 512,
      "chapter_id": 85,
      "position": 59,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:45.000Z",
      "created_at": "2016-10-26T10:35:44.886Z",
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
          "id": 123,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 124,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 515,
      "chapter_id": 86,
      "position": 60,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:45.271Z",
      "created_at": "2016-10-26T10:35:45.157Z",
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
          "id": 125,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 126,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 521,
      "chapter_id": 88,
      "position": 62,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:45.811Z",
      "created_at": "2016-10-26T10:35:45.698Z",
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
          "id": 129,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 130,
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
	-H "Authorization: Bearer b1910a2465a82ebdcbe41c10c9f75bd4e8272a8b4cb02eeef570bd800d5237a9"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer fa67b83ef483561a7bab9064b1c371d9728e48fe57e930bcb6185386459cb077
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
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 505,
      "chapter_id": 83,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:44.413Z",
      "created_at": "2016-10-26T10:35:44.303Z",
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
          "id": 119,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 120,
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
	-H "Authorization: Bearer fa67b83ef483561a7bab9064b1c371d9728e48fe57e930bcb6185386459cb077"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/67/republish
Content-Type: application/json
Authorization: Bearer d5472878c0c1f8433f72832d58f7fc26d95642655a1c8ec411a943943db4e4d2
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
	-H "Authorization: Bearer d5472878c0c1f8433f72832d58f7fc26d95642655a1c8ec411a943943db4e4d2"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 141c31992ac2e6f566c5d7f7c7df2586ba865e28f32e51dbfdeae92ab658abb6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":16,"published":false}}
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
    "creator_id": 33,
    "id": 14,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 14,
    "additional_university_ids": [

    ],
    "topic_id": 16,
    "discipline_id": 17,
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
    "updated_at": "2016-10-26T10:35:07.366Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":16,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 141c31992ac2e6f566c5d7f7c7df2586ba865e28f32e51dbfdeae92ab658abb6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1f66d50231c46e38c92ce1d6bb4c9ff3adcb90588a31641cf38cfadf8f382a9d
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
      "creator_id": 61,
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 41,
      "discipline_id": 42,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
      "updated_at": "2016-10-26T10:35:09.898Z",
      "shortname": "fu-course-28"
    },
    {
      "creator_id": 61,
      "id": 40,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-29",
      "html_url": "https://goskive.com/course/fu-course-29",
      "slug": "fu-course-29",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 42,
      "discipline_id": 43,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 29",
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
      "updated_at": "2016-10-26T10:35:09.949Z",
      "shortname": "fu-course-29"
    },
    {
      "creator_id": 62,
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-30",
      "html_url": "https://goskive.com/course/fu-course-30",
      "slug": "fu-course-30",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 43,
      "discipline_id": 44,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 30",
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
      "updated_at": "2016-10-26T10:35:10.010Z",
      "shortname": "fu-course-30"
    },
    {
      "creator_id": 62,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 44,
      "discipline_id": 45,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 31",
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
      "chapters_updated_at": "2016-10-26T10:35:10.306Z",
      "updated_at": "2016-10-26T10:35:10.312Z",
      "shortname": "fu-course-31"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f66d50231c46e38c92ce1d6bb4c9ff3adcb90588a31641cf38cfadf8f382a9d"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 642dba627f0b0afdc3d82069a4480f77e14e5f93279be4d7a56aed07d7454a48
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
      "creator_id": 67,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 45,
      "discipline_id": 46,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
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
      "updated_at": "2016-10-26T10:35:10.481Z",
      "shortname": "fu-course-32"
    },
    {
      "creator_id": 67,
      "id": 44,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-33",
      "html_url": "https://goskive.com/course/fu-course-33",
      "slug": "fu-course-33",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 46,
      "discipline_id": 47,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 33",
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
      "updated_at": "2016-10-26T10:35:10.524Z",
      "shortname": "fu-course-33"
    },
    {
      "creator_id": 68,
      "id": 45,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-34",
      "html_url": "https://goskive.com/course/fu-course-34",
      "slug": "fu-course-34",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 47,
      "discipline_id": 48,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 34",
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
      "updated_at": "2016-10-26T10:35:10.572Z",
      "shortname": "fu-course-34"
    },
    {
      "creator_id": 68,
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-35",
      "html_url": "https://goskive.com/course/fu-course-35",
      "slug": "fu-course-35",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 48,
      "discipline_id": 49,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 35",
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
      "updated_at": "2016-10-26T10:35:10.616Z",
      "shortname": "fu-course-35"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 642dba627f0b0afdc3d82069a4480f77e14e5f93279be4d7a56aed07d7454a48"
```
