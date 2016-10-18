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
DELETE /v2/chapters/114
Content-Type: application/json
Authorization: Bearer 605d3d46b8089485e39fc2db45e190cacd497d03f10e87a758a3fda0e31ed53c
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/114" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 605d3d46b8089485e39fc2db45e190cacd497d03f10e87a758a3fda0e31ed53c"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/117
Content-Type: application/json
Authorization: Bearer 98f3666afc51c1d0c63022f8282a3205798cee034e440b752c79c390bc77be32
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
    "id": 117,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T09:28:36.543Z",
    "course_id": 215,
    "author_id": 627,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T09:28:35.837Z",
    "questions_updated_at": "2016-10-18T09:28:35.837Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 630,
        "chapter_id": 117,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:36.474Z",
        "created_at": "2016-10-18T09:28:36.474Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 631,
        "chapter_id": 117,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:36.519Z",
        "created_at": "2016-10-18T09:28:36.519Z",
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
        "id": 109,
        "obfuscated_id": "VSPyck5c2RY",
        "author_id": 628,
        "chapter_id": 117,
        "position": 96,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:36.102Z",
        "created_at": "2016-10-18T09:28:35.950Z",
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
      },
      {
        "id": 110,
        "obfuscated_id": "55JK4PuG2Hk",
        "author_id": 629,
        "chapter_id": 117,
        "position": 97,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:36.384Z",
        "created_at": "2016-10-18T09:28:36.218Z",
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
            "id": 223,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 224,
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
curl "api.goskive.com/v2/chapters/117" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98f3666afc51c1d0c63022f8282a3205798cee034e440b752c79c390bc77be32"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/111
Content-Type: application/json
Authorization: Bearer b0177f49ad21c34c2ff189d6922674afc0635a27b21944ad2efcb2480404e36d
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
    "id": 111,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T09:28:34.572Z",
    "course_id": 209,
    "author_id": 609,
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
curl "api.goskive.com/v2/chapters/111" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0177f49ad21c34c2ff189d6922674afc0635a27b21944ad2efcb2480404e36d"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/1
Content-Type: application/json
Authorization: Bearer 45607149574701a1adfdbe161206791cf8760a4a30f25ae233dd9a4196e9f655
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45607149574701a1adfdbe161206791cf8760a4a30f25ae233dd9a4196e9f655"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c67cec881c3d0bc83772d0224a3cf30a710928befe5eaf84965cae1fbb06b3e3
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
      "id": 11,
      "author_id": 127,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:46.527Z",
      "status": "published",
      "subject_id": 70,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 129,
      "reply_to_id": 11,
      "created_at": "2016-10-18T09:27:46.612Z",
      "status": "published",
      "subject_id": 71,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 131,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:46.693Z",
      "status": "published",
      "subject_id": 72,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 133,
      "reply_to_id": 13,
      "created_at": "2016-10-18T09:27:46.774Z",
      "status": "published",
      "subject_id": 73,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 135,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:46.856Z",
      "status": "reported",
      "subject_id": 74,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 137,
      "reply_to_id": 15,
      "created_at": "2016-10-18T09:27:46.935Z",
      "status": "published",
      "subject_id": 75,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 139,
      "reply_to_id": 15,
      "created_at": "2016-10-18T09:27:47.043Z",
      "status": "published",
      "subject_id": 76,
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
	-H "Authorization: Bearer c67cec881c3d0bc83772d0224a3cf30a710928befe5eaf84965cae1fbb06b3e3"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c7b8ff149c2fac7efde277b219eae0ad6612a37eed46d57f5e12965cb5080262
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
      "id": 32,
      "author_id": 172,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:48.437Z",
      "status": "published",
      "subject_id": 91,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 174,
      "reply_to_id": 32,
      "created_at": "2016-10-18T09:27:48.520Z",
      "status": "published",
      "subject_id": 92,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 176,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:48.601Z",
      "status": "published",
      "subject_id": 93,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 178,
      "reply_to_id": 34,
      "created_at": "2016-10-18T09:27:48.682Z",
      "status": "published",
      "subject_id": 94,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 180,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:48.765Z",
      "status": "reported",
      "subject_id": 95,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 182,
      "reply_to_id": 36,
      "created_at": "2016-10-18T09:27:48.847Z",
      "status": "published",
      "subject_id": 96,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 184,
      "reply_to_id": 36,
      "created_at": "2016-10-18T09:27:48.929Z",
      "status": "published",
      "subject_id": 97,
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
	-H "Authorization: Bearer c7b8ff149c2fac7efde277b219eae0ad6612a37eed46d57f5e12965cb5080262"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer b4aaa41fd463c35b2bd37bc6472d5ca0557ba3d8acd970b9dc020caae60a549d
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
      "id": 5,
      "author_id": 114,
      "reply_to_id": 4,
      "created_at": "2016-10-18T09:27:45.972Z",
      "status": "published",
      "subject_id": 64,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 118,
      "reply_to_id": 6,
      "created_at": "2016-10-18T09:27:46.137Z",
      "status": "published",
      "subject_id": 66,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 122,
      "reply_to_id": 8,
      "created_at": "2016-10-18T09:27:46.304Z",
      "status": "published",
      "subject_id": 68,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 124,
      "reply_to_id": 8,
      "created_at": "2016-10-18T09:27:46.388Z",
      "status": "published",
      "subject_id": 69,
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
	-H "Authorization: Bearer b4aaa41fd463c35b2bd37bc6472d5ca0557ba3d8acd970b9dc020caae60a549d"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 670e388f0b39cc5fa06e1f463154bf515f0dad5fdc1b3c3c681a274a8043a946
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
      "id": 29,
      "author_id": 165,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:27:48.146Z",
      "status": "reported",
      "subject_id": 88,
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
	-H "Authorization: Bearer 670e388f0b39cc5fa06e1f463154bf515f0dad5fdc1b3c3c681a274a8043a946"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/39/republish
Content-Type: application/json
Authorization: Bearer 5bad7970d2499b13e76fb444c07b682ebab0c4b80820efbe81c8dd17a9b63476
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/39/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bad7970d2499b13e76fb444c07b682ebab0c4b80820efbe81c8dd17a9b63476"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/281/chapters
Content-Type: application/json
Authorization: Bearer adf5e3aa7731e2595c9cbfa18b127b96e6b07be474e8d012851100a17850153f
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
    "id": 166,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:28:55.268Z",
    "course_id": 281,
    "author_id": 872,
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
curl "api.goskive.com/v2/courses/281/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adf5e3aa7731e2595c9cbfa18b127b96e6b07be474e8d012851100a17850153f"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fda1ee194565bb9e6353e4ea43f8a1c3efb64cb3951cf466ab4336bebd28ba11
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
    "id": 168,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:28:55.654Z",
    "course_id": 284,
    "author_id": 878,
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
	-H "Authorization: Bearer fda1ee194565bb9e6353e4ea43f8a1c3efb64cb3951cf466ab4336bebd28ba11"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b614b9271a312c59dec140148f66f37ae416827788dff7bc98e6c9e45b01875d
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
      "id": 184,
      "title": "Clever Chapter Title 160",
      "position": 1,
      "updated_at": "2016-10-18T09:28:57.802Z",
      "course_id": 293,
      "author_id": 912,
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
      "id": 185,
      "title": "Clever Chapter Title 161",
      "position": 2,
      "updated_at": "2016-10-18T09:28:57.834Z",
      "course_id": 293,
      "author_id": 913,
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
      "id": 186,
      "title": "Clever Chapter Title 162",
      "position": 3,
      "updated_at": "2016-10-18T09:28:58.208Z",
      "course_id": 293,
      "author_id": 914,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T09:28:57.725Z",
      "questions_updated_at": "2016-10-18T09:28:57.725Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b614b9271a312c59dec140148f66f37ae416827788dff7bc98e6c9e45b01875d"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 995ad950a18080784e0ea59e328e07480979fbf236d6b5a2823655bb7eeb048b
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
      "id": 187,
      "title": "Clever Chapter Title 163",
      "position": 1,
      "updated_at": "2016-10-18T09:28:58.475Z",
      "course_id": 295,
      "author_id": 921,
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
      "id": 188,
      "title": "Clever Chapter Title 164",
      "position": 2,
      "updated_at": "2016-10-18T09:28:58.500Z",
      "course_id": 295,
      "author_id": 922,
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
      "id": 189,
      "title": "Clever Chapter Title 165",
      "position": 3,
      "updated_at": "2016-10-18T09:28:58.527Z",
      "course_id": 295,
      "author_id": 923,
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
	-H "Authorization: Bearer 995ad950a18080784e0ea59e328e07480979fbf236d6b5a2823655bb7eeb048b"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/113
Content-Type: application/json
Authorization: Bearer 9eae03d0277e3872fe23eb010342e18b9db9c131e9f599d28c93b98eb89d1b99
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/113" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9eae03d0277e3872fe23eb010342e18b9db9c131e9f599d28c93b98eb89d1b99"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 071a33c08e9b45090af058123eae42fbf7c66130aeea41403ba8d32bd2daa27b
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
	-H "Authorization: Bearer 071a33c08e9b45090af058123eae42fbf7c66130aeea41403ba8d32bd2daa27b"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b815ee68a8dcbabb7730ecbd6daf896951d4750b21047319e9d5b6d56268dfb4
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
    "creator_id": 222,
    "id": 109,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 89,
    "additional_university_ids": [

    ],
    "topic_id": 111,
    "discipline_id": 111,
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
    "chapters_updated_at": "2016-10-18T09:27:53.002Z",
    "updated_at": "2016-10-18T09:27:54.527Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 23,
        "title": "Clever Chapter Title 17",
        "position": 1,
        "updated_at": "2016-10-18T09:27:54.477Z",
        "course_id": 109,
        "author_id": 222,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T09:27:53.002Z",
        "questions_updated_at": "2016-10-18T09:27:53.002Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 24,
        "title": "Clever Chapter Title 18",
        "position": 2,
        "updated_at": "2016-10-18T09:27:54.519Z",
        "course_id": 109,
        "author_id": 222,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T09:27:53.002Z",
        "questions_updated_at": "2016-10-18T09:27:53.002Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 222,
        "chapter_id": 23,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.305Z",
        "created_at": "2016-10-18T09:27:54.305Z",
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
        "author_id": 222,
        "chapter_id": 24,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.378Z",
        "created_at": "2016-10-18T09:27:54.378Z",
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
        "author_id": 222,
        "chapter_id": 23,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.346Z",
        "created_at": "2016-10-18T09:27:54.346Z",
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
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 222,
        "chapter_id": 24,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.423Z",
        "created_at": "2016-10-18T09:27:54.423Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 225,
        "chapter_id": 23,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.466Z",
        "created_at": "2016-10-18T09:27:54.466Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 226,
        "chapter_id": 24,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.508Z",
        "created_at": "2016-10-18T09:27:54.508Z",
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
	-H "Authorization: Bearer b815ee68a8dcbabb7730ecbd6daf896951d4750b21047319e9d5b6d56268dfb4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/104
Content-Type: application/json
Authorization: Bearer 8d8e72b88b5bc4a9231d4279835a1dee9b3b43c5cf298cf0638ed0fe247804e9
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
    "creator_id": 210,
    "id": 104,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 84,
    "additional_university_ids": [

    ],
    "topic_id": 106,
    "discipline_id": 106,
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
    "updated_at": "2016-10-18T09:27:51.068Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/104" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d8e72b88b5bc4a9231d4279835a1dee9b3b43c5cf298cf0638ed0fe247804e9"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f8a89e1fa84eabc91e78f13487152ff7b224a3713ca735e2fbe3926d20823977
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
    "creator_id": 213,
    "id": 106,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 86,
    "additional_university_ids": [

    ],
    "topic_id": 108,
    "discipline_id": 108,
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
    "updated_at": "2016-10-18T09:27:51.330Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8a89e1fa84eabc91e78f13487152ff7b224a3713ca735e2fbe3926d20823977"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer cd12329c68c149e71913de573004f5942fb26405e69b29473c838a5fed490bc0
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
      "id": 23,
      "user_id": 525,
      "feedbackable_id": 86,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:25.997Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 529,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:26.342Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 533,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:26.685Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 537,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:27.084Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 541,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T09:28:27.452Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd12329c68c149e71913de573004f5942fb26405e69b29473c838a5fed490bc0"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 3b1856b8a9b509aa2b5f51b8123a7afd7efd23a00a720af01dfb4ff4e3966bd7
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
      "id": 22,
      "user_id": 520,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T09:28:25.620Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b1856b8a9b509aa2b5f51b8123a7afd7efd23a00a720af01dfb4ff4e3966bd7"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Authorization: Bearer dc53731a5e8e692caf2bfb8e7c1348c1a25f0afdcb382f7c2d14bf2e56efd04d
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Authorization: Bearer dc53731a5e8e692caf2bfb8e7c1348c1a25f0afdcb382f7c2d14bf2e56efd04d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/85/feedbacks
Content-Type: application/json
Authorization: Bearer fa40876244d8e4de0d9177498758e7869ddf9a91598ddd298e44cd0f4344141e
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
      "user_id": 843,
      "feedbackable_id": 85,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:53.192Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 842,
      "feedbackable_id": 85,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:53.180Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/85/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa40876244d8e4de0d9177498758e7869ddf9a91598ddd298e44cd0f4344141e"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5cf88bc4545a3344a47bb06e4c9a181ef6a2e5d0676b5d08d22350dd0c2f32a9
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 773,
      "chapter_id": 140,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:49.021Z",
      "created_at": "2016-10-18T09:28:49.021Z",
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 776,
      "chapter_id": 141,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:49.173Z",
      "created_at": "2016-10-18T09:28:49.173Z",
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
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 779,
      "chapter_id": 142,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:49.328Z",
      "created_at": "2016-10-18T09:28:49.328Z",
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
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 782,
      "chapter_id": 143,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:49.485Z",
      "created_at": "2016-10-18T09:28:49.485Z",
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 785,
      "chapter_id": 144,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:49.636Z",
      "created_at": "2016-10-18T09:28:49.636Z",
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
	-H "Authorization: Bearer 5cf88bc4545a3344a47bb06e4c9a181ef6a2e5d0676b5d08d22350dd0c2f32a9"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 841432264421758b0c84666ce7376964ee933a69a96d825e68cea0b68b89bef5
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 769,
      "chapter_id": 139,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:48.839Z",
      "created_at": "2016-10-18T09:28:48.839Z",
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
	-H "Authorization: Bearer 841432264421758b0c84666ce7376964ee933a69a96d825e68cea0b68b89bef5"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/75/republish
Content-Type: application/json
Authorization: Bearer 050ee9d725061ba1a31f82747efd96111c662ae883d3245379d11f336bd7a794
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 050ee9d725061ba1a31f82747efd96111c662ae883d3245379d11f336bd7a794"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/47/feedbacks
Content-Type: application/json
Authorization: Bearer 5dd98291bd4c86ee35b8fb6efdcffe57f6111079471f6ae855e76d0843e74657
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
      "id": 4,
      "user_id": 321,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:05.114Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 320,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:05.102Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/47/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5dd98291bd4c86ee35b8fb6efdcffe57f6111079471f6ae855e76d0843e74657"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 482aa89f89c47254dc02b52c4ee37ca99dba3cf8aad4a459cea3e3a7eeefeeb2
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
      "author_id": 416,
      "chapter_id": 69,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:14.863Z",
      "created_at": "2016-10-18T09:28:14.725Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 410,
      "chapter_id": 67,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:14.239Z",
      "created_at": "2016-10-18T09:28:14.101Z",
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
          "id": 144,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 145,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 413,
      "chapter_id": 68,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:14.552Z",
      "created_at": "2016-10-18T09:28:14.413Z",
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
    },
    {
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 419,
      "chapter_id": 70,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:15.174Z",
      "created_at": "2016-10-18T09:28:15.034Z",
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
      "author_id": 422,
      "chapter_id": 71,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:15.479Z",
      "created_at": "2016-10-18T09:28:15.346Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 482aa89f89c47254dc02b52c4ee37ca99dba3cf8aad4a459cea3e3a7eeefeeb2"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer be834ea63f7f5a47a6197322b3163d12d089c88f4e565d560b9fcc1ad01815a9
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
      "author_id": 390,
      "chapter_id": 61,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:12.251Z",
      "created_at": "2016-10-18T09:28:12.123Z",
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
	-H "Authorization: Bearer be834ea63f7f5a47a6197322b3163d12d089c88f4e565d560b9fcc1ad01815a9"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/56/republish
Content-Type: application/json
Authorization: Bearer 4354d6d59eafe3ad897d99295098e69331a2f55ce8eb1aad7e24f16c3a439f64
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4354d6d59eafe3ad897d99295098e69331a2f55ce8eb1aad7e24f16c3a439f64"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9887baba9e6f3a703a3a583a6788f7aabedd9b8486d7af86dc492e30b41d7a16
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":50,"published":false}}
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
    "creator_id": 74,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 29,
    "additional_university_ids": [

    ],
    "topic_id": 50,
    "discipline_id": 50,
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
    "updated_at": "2016-10-18T09:27:42.669Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":50,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9887baba9e6f3a703a3a583a6788f7aabedd9b8486d7af86dc492e30b41d7a16"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 699bbe8d1ebea0c1589e10475bcb4cf3295421e1aac22285f0961f125abec2b8
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
      "creator_id": 41,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-13",
      "html_url": "https://goskive.com/course/fu-course-13",
      "slug": "fu-course-13",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 13",
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
      "updated_at": "2016-10-18T09:27:39.491Z",
      "shortname": "fu-course-13"
    },
    {
      "creator_id": 41,
      "id": 21,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-14",
      "html_url": "https://goskive.com/course/fu-course-14",
      "slug": "fu-course-14",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 21,
      "discipline_id": 21,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 14",
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
      "updated_at": "2016-10-18T09:27:39.530Z",
      "shortname": "fu-course-14"
    },
    {
      "creator_id": 42,
      "id": 22,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 22,
      "discipline_id": 22,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
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
      "updated_at": "2016-10-18T09:27:39.576Z",
      "shortname": "fu-course-15"
    },
    {
      "creator_id": 42,
      "id": 23,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 23,
      "discipline_id": 23,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
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
      "chapters_updated_at": "2016-10-18T09:27:39.860Z",
      "updated_at": "2016-10-18T09:27:39.866Z",
      "shortname": "fu-course-16"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 699bbe8d1ebea0c1589e10475bcb4cf3295421e1aac22285f0961f125abec2b8"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0c97fd259bec0f6673ab6c476ae908d36a6074adca1bdf841dd2c6b382e5bc49
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
      "creator_id": 48,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-17",
      "html_url": "https://goskive.com/course/fu-course-17",
      "slug": "fu-course-17",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 24,
      "discipline_id": 24,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 17",
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
      "updated_at": "2016-10-18T09:27:40.065Z",
      "shortname": "fu-course-17"
    },
    {
      "creator_id": 48,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-18",
      "html_url": "https://goskive.com/course/fu-course-18",
      "slug": "fu-course-18",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 25,
      "discipline_id": 25,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 18",
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
      "updated_at": "2016-10-18T09:27:40.104Z",
      "shortname": "fu-course-18"
    },
    {
      "creator_id": 49,
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 26,
      "discipline_id": 26,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
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
      "updated_at": "2016-10-18T09:27:40.152Z",
      "shortname": "fu-course-19"
    },
    {
      "creator_id": 49,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 27,
      "discipline_id": 27,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
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
      "updated_at": "2016-10-18T09:27:40.192Z",
      "shortname": "fu-course-20"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c97fd259bec0f6673ab6c476ae908d36a6074adca1bdf841dd2c6b382e5bc49"
```
