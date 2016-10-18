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
DELETE /v2/chapters/195
Content-Type: application/json
Authorization: Bearer a5128be4762ae33bd2414da5c7053193b39515dfcb2ed90ecac80439b3e43c7c
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/195" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5128be4762ae33bd2414da5c7053193b39515dfcb2ed90ecac80439b3e43c7c"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 33d17e7460a260a41413e944d1518e736b5e7e56979cba6527682d0006955ebe
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
    "id": 191,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T12:37:41.352Z",
    "course_id": 303,
    "author_id": 944,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T12:37:40.808Z",
    "questions_updated_at": "2016-10-18T12:37:40.808Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 94,
        "obfuscated_id": "CVi6VU_nV6k",
        "author_id": 947,
        "chapter_id": 191,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:41.296Z",
        "created_at": "2016-10-18T12:37:41.296Z",
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
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 948,
        "chapter_id": 191,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:41.335Z",
        "created_at": "2016-10-18T12:37:41.335Z",
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
        "id": 131,
        "obfuscated_id": "gCw8isdgMKE",
        "author_id": 945,
        "chapter_id": 191,
        "position": 118,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:41.032Z",
        "created_at": "2016-10-18T12:37:40.918Z",
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
            "id": 265,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 266,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 132,
        "obfuscated_id": "RECRPLqMrqE",
        "author_id": 946,
        "chapter_id": 191,
        "position": 119,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:41.226Z",
        "created_at": "2016-10-18T12:37:41.107Z",
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
            "id": 267,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 268,
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
curl "api.goskive.com/v2/chapters/191" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33d17e7460a260a41413e944d1518e736b5e7e56979cba6527682d0006955ebe"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 38bbd9bd24f956dc4f94ee01eb992f4cfb4f7cfa905284d701015653fbdef474
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
    "id": 189,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T12:37:40.159Z",
    "course_id": 301,
    "author_id": 934,
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
curl "api.goskive.com/v2/chapters/189" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38bbd9bd24f956dc4f94ee01eb992f4cfb4f7cfa905284d701015653fbdef474"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 1808b20806f0fdc01e97f4d9beba96d3a46188f2f0fd29eada30d64c348aa572
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
	-H "Authorization: Bearer 1808b20806f0fdc01e97f4d9beba96d3a46188f2f0fd29eada30d64c348aa572"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 4bf6e056b666f6cfd8213c5019550a49395722b87ef6076b1de8ee2fdf297a6b
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
      "id": 12,
      "author_id": 47,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:24.281Z",
      "status": "published",
      "subject_id": 15,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 49,
      "reply_to_id": 12,
      "created_at": "2016-10-18T12:36:24.360Z",
      "status": "published",
      "subject_id": 16,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 51,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:24.448Z",
      "status": "published",
      "subject_id": 17,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 53,
      "reply_to_id": 14,
      "created_at": "2016-10-18T12:36:24.562Z",
      "status": "published",
      "subject_id": 18,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 55,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:24.653Z",
      "status": "reported",
      "subject_id": 19,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 57,
      "reply_to_id": 16,
      "created_at": "2016-10-18T12:36:24.742Z",
      "status": "published",
      "subject_id": 20,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 59,
      "reply_to_id": 16,
      "created_at": "2016-10-18T12:36:24.832Z",
      "status": "published",
      "subject_id": 21,
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
	-H "Authorization: Bearer 4bf6e056b666f6cfd8213c5019550a49395722b87ef6076b1de8ee2fdf297a6b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer ccef7f85cf86c11e21cd26f7ecb18aa89b1e0c5b9ffeea7b3cb9497079a4766a
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
      "id": 26,
      "author_id": 77,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:25.684Z",
      "status": "published",
      "subject_id": 29,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 79,
      "reply_to_id": 26,
      "created_at": "2016-10-18T12:36:25.785Z",
      "status": "published",
      "subject_id": 30,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 81,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:25.881Z",
      "status": "published",
      "subject_id": 31,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 83,
      "reply_to_id": 28,
      "created_at": "2016-10-18T12:36:25.973Z",
      "status": "published",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 85,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:26.061Z",
      "status": "reported",
      "subject_id": 33,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 87,
      "reply_to_id": 30,
      "created_at": "2016-10-18T12:36:26.152Z",
      "status": "published",
      "subject_id": 34,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 89,
      "reply_to_id": 30,
      "created_at": "2016-10-18T12:36:26.247Z",
      "status": "published",
      "subject_id": 35,
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
	-H "Authorization: Bearer ccef7f85cf86c11e21cd26f7ecb18aa89b1e0c5b9ffeea7b3cb9497079a4766a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer dfa405b02145e6338a3136c24393e6d43071b961a6c00f8702bd1f268eb4318d
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
      "id": 34,
      "author_id": 94,
      "reply_to_id": 33,
      "created_at": "2016-10-18T12:36:26.507Z",
      "status": "published",
      "subject_id": 37,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 98,
      "reply_to_id": 35,
      "created_at": "2016-10-18T12:36:26.704Z",
      "status": "published",
      "subject_id": 39,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 102,
      "reply_to_id": 37,
      "created_at": "2016-10-18T12:36:26.895Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 104,
      "reply_to_id": 37,
      "created_at": "2016-10-18T12:36:26.998Z",
      "status": "published",
      "subject_id": 42,
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
	-H "Authorization: Bearer dfa405b02145e6338a3136c24393e6d43071b961a6c00f8702bd1f268eb4318d"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 4a6b57bc97fa072c7d7e1343c543f999f5dca13cd465101da5a331f57c9013f3
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
      "id": 9,
      "author_id": 40,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:23.988Z",
      "status": "reported",
      "subject_id": 12,
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
	-H "Authorization: Bearer 4a6b57bc97fa072c7d7e1343c543f999f5dca13cd465101da5a331f57c9013f3"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/41/republish
Content-Type: application/json
Authorization: Bearer 183545972778a27ee83d9a4c31d19bd5dfa89fd8753ff78f64a1d5be7acd01ac
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/41/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 183545972778a27ee83d9a4c31d19bd5dfa89fd8753ff78f64a1d5be7acd01ac"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8e09d0bfeb55d65dd1307107d359167cd7a307e091819c481b56993f205c2358
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
    "id": 175,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:37:34.530Z",
    "course_id": 285,
    "author_id": 874,
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
	-H "Authorization: Bearer 8e09d0bfeb55d65dd1307107d359167cd7a307e091819c481b56993f205c2358"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/286/chapters
Content-Type: application/json
Authorization: Bearer c695168cfde6ed866df4e44bf00005ed585e3f32ba7ba700ed33681913b641ea
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
    "id": 176,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:37:34.681Z",
    "course_id": 286,
    "author_id": 876,
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
curl "api.goskive.com/v2/courses/286/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c695168cfde6ed866df4e44bf00005ed585e3f32ba7ba700ed33681913b641ea"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 81f4d2cf056f3e813bd13cf39343c36ddf76b94fcf07e8aa6ec478d7100e3651
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
      "id": 153,
      "title": "Clever Chapter Title 141",
      "position": 1,
      "updated_at": "2016-10-18T12:37:31.484Z",
      "course_id": 272,
      "author_id": 824,
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
      "id": 154,
      "title": "Clever Chapter Title 142",
      "position": 2,
      "updated_at": "2016-10-18T12:37:31.514Z",
      "course_id": 272,
      "author_id": 825,
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
      "id": 155,
      "title": "Clever Chapter Title 143",
      "position": 3,
      "updated_at": "2016-10-18T12:37:31.829Z",
      "course_id": 272,
      "author_id": 826,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T12:37:31.406Z",
      "questions_updated_at": "2016-10-18T12:37:31.406Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81f4d2cf056f3e813bd13cf39343c36ddf76b94fcf07e8aa6ec478d7100e3651"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer dcdf4d064a55d8d651510083a8cb506b3859707be8cb91d5a01d6bee9978ddd8
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
      "id": 156,
      "title": "Clever Chapter Title 144",
      "position": 1,
      "updated_at": "2016-10-18T12:37:32.124Z",
      "course_id": 274,
      "author_id": 833,
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
      "id": 157,
      "title": "Clever Chapter Title 145",
      "position": 2,
      "updated_at": "2016-10-18T12:37:32.155Z",
      "course_id": 274,
      "author_id": 834,
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
      "id": 158,
      "title": "Clever Chapter Title 146",
      "position": 3,
      "updated_at": "2016-10-18T12:37:32.185Z",
      "course_id": 274,
      "author_id": 835,
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
	-H "Authorization: Bearer dcdf4d064a55d8d651510083a8cb506b3859707be8cb91d5a01d6bee9978ddd8"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f177c6d96b69854af87f91425726b9521009674f7bdec057e3451547e5cf8497
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
	-H "Authorization: Bearer f177c6d96b69854af87f91425726b9521009674f7bdec057e3451547e5cf8497"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/188
Content-Type: application/json
Authorization: Bearer 0ad1a4086b3e8fa5dbfb09512815e5f8fb04982634a0b55ff9fdd7e26c0054ec
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/188" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ad1a4086b3e8fa5dbfb09512815e5f8fb04982634a0b55ff9fdd7e26c0054ec"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 3f173c6b1624a14ba886076ee3474fb781bfb8dc44dd1c8d54464088d78cc145
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
    "creator_id": 545,
    "id": 192,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 170,
    "additional_university_ids": [

    ],
    "topic_id": 200,
    "discipline_id": 200,
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
    "chapters_updated_at": "2016-10-18T12:37:07.815Z",
    "updated_at": "2016-10-18T12:37:09.521Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 96,
        "title": "Clever Chapter Title 90",
        "position": 1,
        "updated_at": "2016-10-18T12:37:09.468Z",
        "course_id": 192,
        "author_id": 545,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T12:37:07.815Z",
        "questions_updated_at": "2016-10-18T12:37:07.815Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 97,
        "title": "Clever Chapter Title 91",
        "position": 2,
        "updated_at": "2016-10-18T12:37:09.512Z",
        "course_id": 192,
        "author_id": 545,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T12:37:07.815Z",
        "questions_updated_at": "2016-10-18T12:37:07.815Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 545,
        "chapter_id": 96,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.285Z",
        "created_at": "2016-10-18T12:37:09.285Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 545,
        "chapter_id": 97,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.364Z",
        "created_at": "2016-10-18T12:37:09.364Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 545,
        "chapter_id": 96,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.329Z",
        "created_at": "2016-10-18T12:37:09.329Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 545,
        "chapter_id": 97,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.411Z",
        "created_at": "2016-10-18T12:37:09.411Z",
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
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 548,
        "chapter_id": 96,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.456Z",
        "created_at": "2016-10-18T12:37:09.456Z",
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
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 549,
        "chapter_id": 97,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:09.501Z",
        "created_at": "2016-10-18T12:37:09.501Z",
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
	-H "Authorization: Bearer 3f173c6b1624a14ba886076ee3474fb781bfb8dc44dd1c8d54464088d78cc145"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/175
Content-Type: application/json
Authorization: Bearer 55d96a99775e5bc57bdb0a2973614f1737c10f3db3a9accace8237792a5e9132
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
    "creator_id": 499,
    "id": 175,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 153,
    "additional_university_ids": [

    ],
    "topic_id": 183,
    "discipline_id": 183,
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
    "updated_at": "2016-10-18T12:37:00.372Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/175" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55d96a99775e5bc57bdb0a2973614f1737c10f3db3a9accace8237792a5e9132"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 28ae1b90e1ca5c773c52f5ad15b0ecda26c86f5752e49f689ba4876bbe8d6170
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
    "creator_id": 502,
    "id": 177,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 155,
    "additional_university_ids": [

    ],
    "topic_id": 185,
    "discipline_id": 185,
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
    "updated_at": "2016-10-18T12:37:00.653Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28ae1b90e1ca5c773c52f5ad15b0ecda26c86f5752e49f689ba4876bbe8d6170"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer d8884279dd33f2f9189a309efd755a7a09b22eddd15b1c8bec722340f573c63d
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
      "id": 10,
      "user_id": 240,
      "feedbackable_id": 35,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:39.985Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 244,
      "feedbackable_id": 36,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:40.278Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 248,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:40.576Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 252,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:40.896Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 256,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T12:36:41.214Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8884279dd33f2f9189a309efd755a7a09b22eddd15b1c8bec722340f573c63d"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer ca88abbe1c05f4061adde890b8676b337770cee14e5db653f4aaf236bacf6afb
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
      "user_id": 277,
      "feedbackable_id": 44,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T12:36:42.855Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca88abbe1c05f4061adde890b8676b337770cee14e5db653f4aaf236bacf6afb"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 1ba605870d36997a1156b47f11f5f9b013de4a1f94bb4197f18de1cdf74d73c6
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
	-H "Authorization: Bearer 1ba605870d36997a1156b47f11f5f9b013de4a1f94bb4197f18de1cdf74d73c6" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/57/feedbacks
Content-Type: application/json
Authorization: Bearer 243e611f620b24f468c054440753fd6e96dc75ca1ab401791e854dc868e94f44
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
      "user_id": 603,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:37:13.970Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 602,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:37:13.959Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 243e611f620b24f468c054440753fd6e96dc75ca1ab401791e854dc868e94f44"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 11aff58da86c395d983c4ebb965ec7935af760c10c44aacdac94bbf2075fcb07
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 743,
      "chapter_id": 134,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.325Z",
      "created_at": "2016-10-18T12:37:26.325Z",
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
      "author_id": 746,
      "chapter_id": 135,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.478Z",
      "created_at": "2016-10-18T12:37:26.478Z",
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
      "author_id": 749,
      "chapter_id": 136,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.633Z",
      "created_at": "2016-10-18T12:37:26.633Z",
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
      "author_id": 752,
      "chapter_id": 137,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.780Z",
      "created_at": "2016-10-18T12:37:26.780Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 755,
      "chapter_id": 138,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.940Z",
      "created_at": "2016-10-18T12:37:26.940Z",
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
	-H "Authorization: Bearer 11aff58da86c395d983c4ebb965ec7935af760c10c44aacdac94bbf2075fcb07"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 1356fe1e7622b9ed00f744ba9734d723d55ef09c6b47001b86a8c05eb8f9634f
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 739,
      "chapter_id": 133,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:26.122Z",
      "created_at": "2016-10-18T12:37:26.122Z",
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
	-H "Authorization: Bearer 1356fe1e7622b9ed00f744ba9734d723d55ef09c6b47001b86a8c05eb8f9634f"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/82/republish
Content-Type: application/json
Authorization: Bearer a5d7d716ba4561605280dfb43a093f7cabd9a73415798677cdb280d0224aba89
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/82/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5d7d716ba4561605280dfb43a093f7cabd9a73415798677cdb280d0224aba89"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/58/feedbacks
Content-Type: application/json
Authorization: Bearer 134f6ab878f22158b1d10156ec16b806cbadc6ef475127c393589e1c1d925bc5
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
      "user_id": 437,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:55.297Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 436,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:55.284Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/58/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 134f6ab878f22158b1d10156ec16b806cbadc6ef475127c393589e1c1d925bc5"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 9728952a4ae678816595ec89889930c5a480e0dce9d693d6d37c6e4a5d41f7ad
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 162,
      "chapter_id": 18,
      "position": 10,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:32.846Z",
      "created_at": "2016-10-18T12:36:32.723Z",
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
    },
    {
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 153,
      "chapter_id": 15,
      "position": 7,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:31.990Z",
      "created_at": "2016-10-18T12:36:31.872Z",
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
      "author_id": 156,
      "chapter_id": 16,
      "position": 8,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:32.277Z",
      "created_at": "2016-10-18T12:36:32.156Z",
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 159,
      "chapter_id": 17,
      "position": 9,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:32.562Z",
      "created_at": "2016-10-18T12:36:32.440Z",
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 165,
      "chapter_id": 19,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:33.121Z",
      "created_at": "2016-10-18T12:36:33.006Z",
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
          "id": 32,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 33,
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
	-H "Authorization: Bearer 9728952a4ae678816595ec89889930c5a480e0dce9d693d6d37c6e4a5d41f7ad"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer b3e371611edfb5274349bcaab4564f1a0b90046c0e3943ff3ff90f4479060711
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 149,
      "chapter_id": 14,
      "position": 6,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:31.662Z",
      "created_at": "2016-10-18T12:36:31.542Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3e371611edfb5274349bcaab4564f1a0b90046c0e3943ff3ff90f4479060711"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/5/republish
Content-Type: application/json
Authorization: Bearer 2cf627872a4d0c06684a64844cbd18680e3fb75b21b6e8ecd896412009ff5eba
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
	-H "Authorization: Bearer 2cf627872a4d0c06684a64844cbd18680e3fb75b21b6e8ecd896412009ff5eba"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 02de7c3cfbf440df1bffac142a496b958ceefc88284d01f0419c148aa776ce5a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":104,"published":false}}
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
    "creator_id": 329,
    "id": 101,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 101,
    "additional_university_ids": [

    ],
    "topic_id": 104,
    "discipline_id": 104,
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
    "updated_at": "2016-10-18T12:36:45.973Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":104,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02de7c3cfbf440df1bffac142a496b958ceefc88284d01f0419c148aa776ce5a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8ec9f378f4c34663e2a0ce317b5387250c6ec224f09904f2fc91732ba54c1dcd
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
      "creator_id": 363,
      "id": 132,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 135,
      "discipline_id": 135,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
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
      "updated_at": "2016-10-18T12:36:49.424Z",
      "shortname": "fu-course-128"
    },
    {
      "creator_id": 363,
      "id": 133,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-129",
      "html_url": "https://goskive.com/course/fu-course-129",
      "slug": "fu-course-129",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 136,
      "discipline_id": 136,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 129",
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
      "updated_at": "2016-10-18T12:36:49.464Z",
      "shortname": "fu-course-129"
    },
    {
      "creator_id": 364,
      "id": 134,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 137,
      "discipline_id": 137,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 130",
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
      "updated_at": "2016-10-18T12:36:49.513Z",
      "shortname": "fu-course-130"
    },
    {
      "creator_id": 364,
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 138,
      "discipline_id": 138,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
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
      "chapters_updated_at": "2016-10-18T12:36:49.816Z",
      "updated_at": "2016-10-18T12:36:49.823Z",
      "shortname": "fu-course-131"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ec9f378f4c34663e2a0ce317b5387250c6ec224f09904f2fc91732ba54c1dcd"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 18d5372db0e00af78d829cc90e5ac3a778afbcb8bb363f8eb2d483aac0dffd3b
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
      "creator_id": 369,
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 139,
      "discipline_id": 139,
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
      "updated_at": "2016-10-18T12:36:49.971Z",
      "shortname": "fu-course-132"
    },
    {
      "creator_id": 369,
      "id": 137,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-133",
      "html_url": "https://goskive.com/course/fu-course-133",
      "slug": "fu-course-133",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 140,
      "discipline_id": 140,
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
      "updated_at": "2016-10-18T12:36:50.012Z",
      "shortname": "fu-course-133"
    },
    {
      "creator_id": 370,
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 141,
      "discipline_id": 141,
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
      "updated_at": "2016-10-18T12:36:50.061Z",
      "shortname": "fu-course-134"
    },
    {
      "creator_id": 370,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 142,
      "discipline_id": 142,
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
      "updated_at": "2016-10-18T12:36:50.102Z",
      "shortname": "fu-course-135"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18d5372db0e00af78d829cc90e5ac3a778afbcb8bb363f8eb2d483aac0dffd3b"
```
