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
DELETE /v2/chapters/76
Content-Type: application/json
Authorization: Bearer bc3ce746f6b883f31c170acea30375b03802914f3808391998a7678784fbd4a2
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/76" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc3ce746f6b883f31c170acea30375b03802914f3808391998a7678784fbd4a2"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/79
Content-Type: application/json
Authorization: Bearer 36b57aad8d0e9de9ffa64c1cb89bfe3a9d1aa111cc20d6e7448a304272e26b57
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
    "id": 79,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T13:15:04.343Z",
    "course_id": 134,
    "author_id": 422,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-19T13:15:03.701Z",
    "questions_updated_at": "2016-10-19T13:15:03.701Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 425,
        "chapter_id": 79,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:04.278Z",
        "created_at": "2016-10-19T13:15:04.278Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 426,
        "chapter_id": 79,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:04.322Z",
        "created_at": "2016-10-19T13:15:04.322Z",
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
        "author_id": 423,
        "chapter_id": 79,
        "position": 69,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:03.961Z",
        "created_at": "2016-10-19T13:15:03.827Z",
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
            "id": 137,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 138,
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
        "author_id": 424,
        "chapter_id": 79,
        "position": 70,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:04.195Z",
        "created_at": "2016-10-19T13:15:04.046Z",
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
            "id": 139,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 140,
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
curl "api.goskive.com/v2/chapters/79" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36b57aad8d0e9de9ffa64c1cb89bfe3a9d1aa111cc20d6e7448a304272e26b57"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/80
Content-Type: application/json
Authorization: Bearer b5529706de481a1453f4729a7a13efb1717b192a1b650ba5e8828d095c9a2015
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
    "id": 80,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T13:15:04.591Z",
    "course_id": 135,
    "author_id": 429,
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
curl "api.goskive.com/v2/chapters/80" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5529706de481a1453f4729a7a13efb1717b192a1b650ba5e8828d095c9a2015"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer 213940af0159b4b2583ad14fa1ca826e1f597f8a37ad87d8569d12936a6c865e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 213940af0159b4b2583ad14fa1ca826e1f597f8a37ad87d8569d12936a6c865e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c2306f1d6b8842bb63bc513beef9fc44f41c4290d25deab20d086b07afef363d
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
      "id": 21,
      "author_id": 105,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:33.451Z",
      "status": "published",
      "subject_id": 36,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 107,
      "reply_to_id": 21,
      "created_at": "2016-10-19T13:14:33.540Z",
      "status": "published",
      "subject_id": 37,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 109,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:33.628Z",
      "status": "published",
      "subject_id": 38,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 111,
      "reply_to_id": 23,
      "created_at": "2016-10-19T13:14:33.714Z",
      "status": "published",
      "subject_id": 39,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 113,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:33.801Z",
      "status": "reported",
      "subject_id": 40,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 115,
      "reply_to_id": 25,
      "created_at": "2016-10-19T13:14:33.887Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 117,
      "reply_to_id": 25,
      "created_at": "2016-10-19T13:14:33.980Z",
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
curl "api.goskive.com/v2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2306f1d6b8842bb63bc513beef9fc44f41c4290d25deab20d086b07afef363d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 870cd87ed780b7c524f1da41d1861b40fc92af5be823d6b076b5c0d08f6c3401
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
      "author_id": 120,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:34.152Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 122,
      "reply_to_id": 28,
      "created_at": "2016-10-19T13:14:34.261Z",
      "status": "published",
      "subject_id": 44,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 124,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:34.363Z",
      "status": "published",
      "subject_id": 45,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 126,
      "reply_to_id": 30,
      "created_at": "2016-10-19T13:14:34.467Z",
      "status": "published",
      "subject_id": 46,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 128,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:34.561Z",
      "status": "reported",
      "subject_id": 47,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 130,
      "reply_to_id": 32,
      "created_at": "2016-10-19T13:14:34.650Z",
      "status": "published",
      "subject_id": 48,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 132,
      "reply_to_id": 32,
      "created_at": "2016-10-19T13:14:34.735Z",
      "status": "published",
      "subject_id": 49,
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
	-H "Authorization: Bearer 870cd87ed780b7c524f1da41d1861b40fc92af5be823d6b076b5c0d08f6c3401"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 0da175e670fc6b40b21c6d225dee0450f6bb31760b2974b95cf0368406f4a3cd
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
      "id": 36,
      "author_id": 137,
      "reply_to_id": 35,
      "created_at": "2016-10-19T13:14:34.976Z",
      "status": "published",
      "subject_id": 51,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 141,
      "reply_to_id": 37,
      "created_at": "2016-10-19T13:14:35.165Z",
      "status": "published",
      "subject_id": 53,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 145,
      "reply_to_id": 39,
      "created_at": "2016-10-19T13:14:35.381Z",
      "status": "published",
      "subject_id": 55,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 147,
      "reply_to_id": 39,
      "created_at": "2016-10-19T13:14:35.475Z",
      "status": "published",
      "subject_id": 56,
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
	-H "Authorization: Bearer 0da175e670fc6b40b21c6d225dee0450f6bb31760b2974b95cf0368406f4a3cd"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 84d3db380ea469125a935deacf12d17285636654ccb1d4ba2a8d7788d76bfe16
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
      "id": 11,
      "author_id": 83,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:32.447Z",
      "status": "reported",
      "subject_id": 26,
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
	-H "Authorization: Bearer 84d3db380ea469125a935deacf12d17285636654ccb1d4ba2a8d7788d76bfe16"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/43/republish
Content-Type: application/json
Authorization: Bearer 8a8313ce60dcb1fb25b1bf6a8d92f81c8ff6f87ea7af71381f0f2d12195daa6b
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/43/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a8313ce60dcb1fb25b1bf6a8d92f81c8ff6f87ea7af71381f0f2d12195daa6b"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/125/chapters
Content-Type: application/json
Authorization: Bearer b762bf625ccd035e4dd3f0f52ee1d1d8ff0ad90baadb360d02ef1603a2270298
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
    "id": 71,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T13:15:01.365Z",
    "course_id": 125,
    "author_id": 395,
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
curl "api.goskive.com/v2/courses/125/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b762bf625ccd035e4dd3f0f52ee1d1d8ff0ad90baadb360d02ef1603a2270298"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b7b6d02b8fc3d58d65958af6165f0639e3bdff0dd2cf65ce6bc6c7684e6afb61
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
    "id": 72,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T13:15:01.654Z",
    "course_id": 127,
    "author_id": 399,
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
	-H "Authorization: Bearer b7b6d02b8fc3d58d65958af6165f0639e3bdff0dd2cf65ce6bc6c7684e6afb61"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 30724325585dc95e03de9735b1d7b3fce7308fe24bad1493b2f67c54eac07671
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
      "id": 59,
      "title": "Clever Chapter Title 59",
      "position": 1,
      "updated_at": "2016-10-19T13:14:59.700Z",
      "course_id": 119,
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
      "id": 60,
      "title": "Clever Chapter Title 60",
      "position": 2,
      "updated_at": "2016-10-19T13:14:59.727Z",
      "course_id": 119,
      "author_id": 371,
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
      "id": 61,
      "title": "Clever Chapter Title 61",
      "position": 3,
      "updated_at": "2016-10-19T13:15:00.047Z",
      "course_id": 119,
      "author_id": 372,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-19T13:14:59.621Z",
      "questions_updated_at": "2016-10-19T13:14:59.621Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30724325585dc95e03de9735b1d7b3fce7308fe24bad1493b2f67c54eac07671"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer bb91fedcf1ec06326604546c560f9498f2ed42557aac3c5881782a46186010a4
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
      "id": 62,
      "title": "Clever Chapter Title 62",
      "position": 1,
      "updated_at": "2016-10-19T13:15:00.219Z",
      "course_id": 120,
      "author_id": 377,
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
      "id": 63,
      "title": "Clever Chapter Title 63",
      "position": 2,
      "updated_at": "2016-10-19T13:15:00.254Z",
      "course_id": 120,
      "author_id": 378,
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
      "id": 64,
      "title": "Clever Chapter Title 64",
      "position": 3,
      "updated_at": "2016-10-19T13:15:00.281Z",
      "course_id": 120,
      "author_id": 379,
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
	-H "Authorization: Bearer bb91fedcf1ec06326604546c560f9498f2ed42557aac3c5881782a46186010a4"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/62
Content-Type: application/json
Authorization: Bearer eef1e4275c7f03a89c7eea8344f666b7bed6017ed7d0e65e6e8ce0aacbc6dda1
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/62" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eef1e4275c7f03a89c7eea8344f666b7bed6017ed7d0e65e6e8ce0aacbc6dda1"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer be3c38bbc59012934a2549492742ff750ee7c9ca0b0b265ad50a6679b313797f
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
	-H "Authorization: Bearer be3c38bbc59012934a2549492742ff750ee7c9ca0b0b265ad50a6679b313797f"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer bc7de919fda70258846e23eb947f9b11e6e695072d1a037c3445c5e9c557cfb2
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
    "creator_id": 195,
    "id": 76,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 76,
    "additional_university_ids": [

    ],
    "topic_id": 81,
    "discipline_id": 81,
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
    "chapters_updated_at": "2016-10-19T13:14:40.062Z",
    "updated_at": "2016-10-19T13:14:41.584Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 13,
        "title": "Clever Chapter Title 13",
        "position": 1,
        "updated_at": "2016-10-19T13:14:41.529Z",
        "course_id": 76,
        "author_id": 195,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T13:14:40.062Z",
        "questions_updated_at": "2016-10-19T13:14:40.062Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 14,
        "title": "Clever Chapter Title 14",
        "position": 2,
        "updated_at": "2016-10-19T13:14:41.575Z",
        "course_id": 76,
        "author_id": 195,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T13:14:40.062Z",
        "questions_updated_at": "2016-10-19T13:14:40.062Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 195,
        "chapter_id": 13,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.353Z",
        "created_at": "2016-10-19T13:14:41.353Z",
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
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 195,
        "chapter_id": 14,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.431Z",
        "created_at": "2016-10-19T13:14:41.431Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 195,
        "chapter_id": 13,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.397Z",
        "created_at": "2016-10-19T13:14:41.397Z",
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
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 195,
        "chapter_id": 14,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.473Z",
        "created_at": "2016-10-19T13:14:41.473Z",
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
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 198,
        "chapter_id": 13,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.517Z",
        "created_at": "2016-10-19T13:14:41.517Z",
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
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 199,
        "chapter_id": 14,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.564Z",
        "created_at": "2016-10-19T13:14:41.564Z",
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
	-H "Authorization: Bearer bc7de919fda70258846e23eb947f9b11e6e695072d1a037c3445c5e9c557cfb2"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/71
Content-Type: application/json
Authorization: Bearer a6904937e8b91a2b28116e35494f91beea0ae8780c28725e9282d706c419d77a
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
    "creator_id": 182,
    "id": 71,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 71,
    "additional_university_ids": [

    ],
    "topic_id": 76,
    "discipline_id": 76,
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
    "updated_at": "2016-10-19T13:14:37.967Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/71" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6904937e8b91a2b28116e35494f91beea0ae8780c28725e9282d706c419d77a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4568e2a3eaf01f25a1ec20b70062257606f82b8effb132142a1f04927ba24d52
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
    "creator_id": 185,
    "id": 73,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 73,
    "additional_university_ids": [

    ],
    "topic_id": 78,
    "discipline_id": 78,
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
    "updated_at": "2016-10-19T13:14:38.254Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4568e2a3eaf01f25a1ec20b70062257606f82b8effb132142a1f04927ba24d52"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 08b75e01301cd170260ad3e072a7b4dfa56ecf469f180f0266f7e7b3e953ed3d
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
      "user_id": 743,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:32.546Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 747,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:32.888Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 751,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:33.241Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 755,
      "feedbackable_id": 94,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:33.584Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 759,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T13:15:33.938Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08b75e01301cd170260ad3e072a7b4dfa56ecf469f180f0266f7e7b3e953ed3d"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer f14850708adb691a14ad345d2fd9b693629cf0aeaad3885cc04699ea0c81ce72
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
      "id": 40,
      "user_id": 817,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T13:15:38.600Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f14850708adb691a14ad345d2fd9b693629cf0aeaad3885cc04699ea0c81ce72"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Content-Type: application/json
Authorization: Bearer 2ae2f313b924cda5507ff7701a191ffd3bf7f070814ab13b4ce2f70d0b188775
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ae2f313b924cda5507ff7701a191ffd3bf7f070814ab13b4ce2f70d0b188775"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 5701cb11dcc015547baefebd80cfee8c2f87e1821b9d9f67fbaabaa09a867298
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
      "id": 51,
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
      "created_at": "2016-10-19T13:14:30.501Z",
      "updated_at": "2016-10-19T13:14:30.501Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-19T13:14:30.576Z",
    "updated_at": "2016-10-19T13:14:30.576Z",
    "course_id": 16,
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5701cb11dcc015547baefebd80cfee8c2f87e1821b9d9f67fbaabaa09a867298"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/51/feedbacks
Content-Type: application/json
Authorization: Bearer a9464868691569fbc187cecdab260c9a84c4c45259ae27c3c6101820c900b6ed
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
      "id": 18,
      "user_id": 474,
      "feedbackable_id": 51,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:07.292Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 473,
      "feedbackable_id": 51,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:07.280Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/51/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9464868691569fbc187cecdab260c9a84c4c45259ae27c3c6101820c900b6ed"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 97f7ad6a5c5afb5b73ba190f2360c04af30c036047408f6e79adf486f5fd82e0
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
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 518,
      "chapter_id": 103,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:11.521Z",
      "created_at": "2016-10-19T13:15:11.521Z",
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
      "author_id": 521,
      "chapter_id": 104,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:11.664Z",
      "created_at": "2016-10-19T13:15:11.664Z",
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
      "author_id": 524,
      "chapter_id": 105,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:11.806Z",
      "created_at": "2016-10-19T13:15:11.806Z",
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
      "author_id": 527,
      "chapter_id": 106,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:11.950Z",
      "created_at": "2016-10-19T13:15:11.950Z",
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
      "author_id": 530,
      "chapter_id": 107,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:12.103Z",
      "created_at": "2016-10-19T13:15:12.103Z",
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
	-H "Authorization: Bearer 97f7ad6a5c5afb5b73ba190f2360c04af30c036047408f6e79adf486f5fd82e0"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 62d15d6361be5181b8f4cc8a36d2f0e4f579883e00aa8ca9a73bd6558c9ebd79
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
      "author_id": 546,
      "chapter_id": 112,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:12.940Z",
      "created_at": "2016-10-19T13:15:12.940Z",
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
	-H "Authorization: Bearer 62d15d6361be5181b8f4cc8a36d2f0e4f579883e00aa8ca9a73bd6558c9ebd79"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/republish
Content-Type: application/json
Authorization: Bearer 179d858a6fe064b48e17d42a8fb7732cced4e0cabf8898dc0e97fad91a5d5f53
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 179d858a6fe064b48e17d42a8fb7732cced4e0cabf8898dc0e97fad91a5d5f53"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/54/feedbacks
Content-Type: application/json
Authorization: Bearer 9f33697bcff2caedaa000be3b121d65c0bfa62bcdeb1277644706113b2c87bee
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
      "id": 6,
      "user_id": 321,
      "feedbackable_id": 54,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:54.715Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 320,
      "feedbackable_id": 54,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:54.697Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/54/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f33697bcff2caedaa000be3b121d65c0bfa62bcdeb1277644706113b2c87bee"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer cdfb6024632a02680ef26315ba5290398c81b4888d82a04874c9f7538617910c
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
      "id": 116,
      "obfuscated_id": "PhHGVKqnHFA",
      "author_id": 894,
      "chapter_id": 174,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:43.810Z",
      "created_at": "2016-10-19T13:15:43.688Z",
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
          "id": 234,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 235,
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
      "author_id": 888,
      "chapter_id": 172,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:43.222Z",
      "created_at": "2016-10-19T13:15:43.106Z",
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
          "id": 230,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 231,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 897,
      "chapter_id": 175,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:44.110Z",
      "created_at": "2016-10-19T13:15:43.982Z",
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
          "id": 236,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 237,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 891,
      "chapter_id": 173,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:43.510Z",
      "created_at": "2016-10-19T13:15:43.391Z",
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
          "id": 232,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 233,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 900,
      "chapter_id": 176,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:44.398Z",
      "created_at": "2016-10-19T13:15:44.281Z",
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
          "id": 238,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 239,
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
	-H "Authorization: Bearer cdfb6024632a02680ef26315ba5290398c81b4888d82a04874c9f7538617910c"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9f2d73b72698c6684b5c84a082d63640e65d803948c57c61a1a2ac2e5fc938ac
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
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 916,
      "chapter_id": 181,
      "position": 116,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:46.290Z",
      "created_at": "2016-10-19T13:15:46.150Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f2d73b72698c6684b5c84a082d63640e65d803948c57c61a1a2ac2e5fc938ac"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/111/republish
Content-Type: application/json
Authorization: Bearer 9caaa3babecc6382f2cdc9a8b66cd545bb35bde5dd844262508e04e0877411ed
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9caaa3babecc6382f2cdc9a8b66cd545bb35bde5dd844262508e04e0877411ed"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7ba28a6ab0e20ca81ddb03be49f989fd9e3fb3f336a554b72563afbb4c7c1c0b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":223,"published":false}}
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
    "creator_id": 641,
    "id": 218,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 196,
    "additional_university_ids": [

    ],
    "topic_id": 223,
    "discipline_id": 223,
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
    "updated_at": "2016-10-19T13:15:22.858Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":223,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ba28a6ab0e20ca81ddb03be49f989fd9e3fb3f336a554b72563afbb4c7c1c0b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c146f70e59c73b1b587d42b7343e1206c3d6abbcc46b93a4dd22e93c278b2288
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
      "creator_id": 603,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "topic_id": 190,
      "discipline_id": 190,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-19T13:15:19.057Z",
      "shortname": "fu-course-134"
    },
    {
      "creator_id": 603,
      "id": 186,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "topic_id": 191,
      "discipline_id": 191,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-19T13:15:19.100Z",
      "shortname": "fu-course-135"
    },
    {
      "creator_id": 604,
      "id": 187,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "topic_id": 192,
      "discipline_id": 192,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-19T13:15:19.150Z",
      "shortname": "fu-course-136"
    },
    {
      "creator_id": 604,
      "id": 188,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "topic_id": 193,
      "discipline_id": 193,
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
      "chapters_updated_at": "2016-10-19T13:15:19.490Z",
      "updated_at": "2016-10-19T13:15:19.498Z",
      "shortname": "fu-course-137"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c146f70e59c73b1b587d42b7343e1206c3d6abbcc46b93a4dd22e93c278b2288"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5472855dcf0f81ecab8179f4b823561b1d59ef3de1c4ae8e5e23e528efb61d8f
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
      "creator_id": 610,
      "id": 189,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 185,
      "additional_university_ids": [

      ],
      "topic_id": 194,
      "discipline_id": 194,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-19T13:15:19.720Z",
      "shortname": "fu-course-138"
    },
    {
      "creator_id": 610,
      "id": 190,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 185,
      "additional_university_ids": [

      ],
      "topic_id": 195,
      "discipline_id": 195,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-19T13:15:19.763Z",
      "shortname": "fu-course-139"
    },
    {
      "creator_id": 611,
      "id": 191,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-140",
      "html_url": "https://goskive.com/course/fu-course-140",
      "slug": "fu-course-140",
      "university_id": 185,
      "additional_university_ids": [

      ],
      "topic_id": 196,
      "discipline_id": 196,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 140",
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
      "updated_at": "2016-10-19T13:15:19.816Z",
      "shortname": "fu-course-140"
    },
    {
      "creator_id": 611,
      "id": 192,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 185,
      "additional_university_ids": [

      ],
      "topic_id": 197,
      "discipline_id": 197,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
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
      "updated_at": "2016-10-19T13:15:19.862Z",
      "shortname": "fu-course-141"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5472855dcf0f81ecab8179f4b823561b1d59ef3de1c4ae8e5e23e528efb61d8f"
```
