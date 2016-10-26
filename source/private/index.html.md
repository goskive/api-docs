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
DELETE /v2/chapters/69
Content-Type: application/json
Authorization: Bearer b425813fdbb7a15c53a79fb50d4e002c72f13fea85bc31ef154416603828f2bf
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/69" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b425813fdbb7a15c53a79fb50d4e002c72f13fea85bc31ef154416603828f2bf"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/65
Content-Type: application/json
Authorization: Bearer 0ca57971ec720a53445802c73e2c156efba4ca4f4a22a6f63c8861bcdb37daea
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
    "id": 65,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T19:31:45.990Z",
    "course_id": 114,
    "author_id": 365,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-26T19:31:45.507Z",
    "questions_updated_at": "2016-10-26T19:31:45.507Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 368,
        "chapter_id": 65,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.941Z",
        "created_at": "2016-10-26T19:31:45.941Z",
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
        "author_id": 369,
        "chapter_id": 65,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.974Z",
        "created_at": "2016-10-26T19:31:45.974Z",
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
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 366,
        "chapter_id": 65,
        "position": 32,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.704Z",
        "created_at": "2016-10-26T19:31:45.603Z",
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
            "id": 74,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 75,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 367,
        "chapter_id": 65,
        "position": 33,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.878Z",
        "created_at": "2016-10-26T19:31:45.769Z",
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
            "id": 76,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 77,
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
curl "api.goskive.com/v2/chapters/65" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ca57971ec720a53445802c73e2c156efba4ca4f4a22a6f63c8861bcdb37daea"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/63
Content-Type: application/json
Authorization: Bearer 8f28ebca11cc5495fd48f2a41b5c82ed8bff659f39f03d5a9de215a85fa6b8fb
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
    "id": 63,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T19:31:44.924Z",
    "course_id": 112,
    "author_id": 355,
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
curl "api.goskive.com/v2/chapters/63" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f28ebca11cc5495fd48f2a41b5c82ed8bff659f39f03d5a9de215a85fa6b8fb"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 04bb18356098de39e943dbefd857ee7ad93920929f2d92481b57b2a96442ddf8
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04bb18356098de39e943dbefd857ee7ad93920929f2d92481b57b2a96442ddf8"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 31ab7ffc10fa814e435b3b17338650446f9ddba5e9bb9f84303e0dc9ccb04c07
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
      "id": 10,
      "author_id": 120,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:30.995Z",
      "status": "published",
      "subject_id": 31,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 122,
      "reply_to_id": 10,
      "created_at": "2016-10-26T19:31:31.070Z",
      "status": "published",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 124,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:31.144Z",
      "status": "published",
      "subject_id": 33,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 126,
      "reply_to_id": 12,
      "created_at": "2016-10-26T19:31:31.217Z",
      "status": "published",
      "subject_id": 34,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 128,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:31.290Z",
      "status": "reported",
      "subject_id": 35,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 130,
      "reply_to_id": 14,
      "created_at": "2016-10-26T19:31:31.361Z",
      "status": "published",
      "subject_id": 36,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 132,
      "reply_to_id": 14,
      "created_at": "2016-10-26T19:31:31.433Z",
      "status": "published",
      "subject_id": 37,
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
	-H "Authorization: Bearer 31ab7ffc10fa814e435b3b17338650446f9ddba5e9bb9f84303e0dc9ccb04c07"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 3cedb449864d5a68e48e34fec063a378bd116bc0e3a1c9f2b9307920a3cfe1df
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
      "author_id": 165,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:32.665Z",
      "status": "published",
      "subject_id": 52,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 167,
      "reply_to_id": 31,
      "created_at": "2016-10-26T19:31:32.739Z",
      "status": "published",
      "subject_id": 53,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 169,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:32.815Z",
      "status": "published",
      "subject_id": 54,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 171,
      "reply_to_id": 33,
      "created_at": "2016-10-26T19:31:32.890Z",
      "status": "published",
      "subject_id": 55,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 173,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:32.965Z",
      "status": "reported",
      "subject_id": 56,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 175,
      "reply_to_id": 35,
      "created_at": "2016-10-26T19:31:33.037Z",
      "status": "published",
      "subject_id": 57,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 177,
      "reply_to_id": 35,
      "created_at": "2016-10-26T19:31:33.108Z",
      "status": "published",
      "subject_id": 58,
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
	-H "Authorization: Bearer 3cedb449864d5a68e48e34fec063a378bd116bc0e3a1c9f2b9307920a3cfe1df"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 2a31ac0e5d1b9250218e593d88d80c437bd9fd50de4192313272ed9778b04701
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
      "id": 18,
      "author_id": 137,
      "reply_to_id": 17,
      "created_at": "2016-10-26T19:31:31.629Z",
      "status": "published",
      "subject_id": 39,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 141,
      "reply_to_id": 19,
      "created_at": "2016-10-26T19:31:31.775Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 145,
      "reply_to_id": 21,
      "created_at": "2016-10-26T19:31:31.920Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 147,
      "reply_to_id": 21,
      "created_at": "2016-10-26T19:31:31.993Z",
      "status": "published",
      "subject_id": 44,
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
	-H "Authorization: Bearer 2a31ac0e5d1b9250218e593d88d80c437bd9fd50de4192313272ed9778b04701"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer b87d423ffffeb2143fc732acb1af404ee638603f3f4c0060d716ab2117b5769c
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
      "id": 42,
      "author_id": 188,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:33.552Z",
      "status": "reported",
      "subject_id": 63,
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
	-H "Authorization: Bearer b87d423ffffeb2143fc732acb1af404ee638603f3f4c0060d716ab2117b5769c"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/8/republish
Content-Type: application/json
Authorization: Bearer a7c0b7fac84e701fb4342d69fd8b15a1ae37c3fb9337f298ba50b061944a0480
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7c0b7fac84e701fb4342d69fd8b15a1ae37c3fb9337f298ba50b061944a0480"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 015cb4170489291d5b48b06173f434e3235f169747e076c259368f2884c43889
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
    "id": 34,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:31:40.576Z",
    "course_id": 93,
    "author_id": 282,
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
	-H "Authorization: Bearer 015cb4170489291d5b48b06173f434e3235f169747e076c259368f2884c43889"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/94/chapters
Content-Type: application/json
Authorization: Bearer 36bc36925573709249fd574be77f8f65c648ecdf8a421f152694b413d8de7694
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
    "id": 35,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:31:40.691Z",
    "course_id": 94,
    "author_id": 284,
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
curl "api.goskive.com/v2/courses/94/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36bc36925573709249fd574be77f8f65c648ecdf8a421f152694b413d8de7694"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f1963f87206a3f760b6b911d5f616696855d4453eb5b5c75576cc57725a7ac74
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
      "id": 39,
      "title": "Clever Chapter Title 27",
      "position": 1,
      "updated_at": "2016-10-26T19:31:41.064Z",
      "course_id": 97,
      "author_id": 293,
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
      "id": 40,
      "title": "Clever Chapter Title 28",
      "position": 2,
      "updated_at": "2016-10-26T19:31:41.085Z",
      "course_id": 97,
      "author_id": 294,
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
      "id": 41,
      "title": "Clever Chapter Title 29",
      "position": 3,
      "updated_at": "2016-10-26T19:31:41.312Z",
      "course_id": 97,
      "author_id": 295,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-26T19:31:40.997Z",
      "questions_updated_at": "2016-10-26T19:31:40.997Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1963f87206a3f760b6b911d5f616696855d4453eb5b5c75576cc57725a7ac74"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 51cce9684842a0c37d3213c0202c267f63c8bbe64b8e0ee8c772842d32237891
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
      "id": 42,
      "title": "Clever Chapter Title 30",
      "position": 1,
      "updated_at": "2016-10-26T19:31:41.448Z",
      "course_id": 98,
      "author_id": 300,
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
      "id": 43,
      "title": "Clever Chapter Title 31",
      "position": 2,
      "updated_at": "2016-10-26T19:31:41.471Z",
      "course_id": 98,
      "author_id": 301,
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
      "id": 44,
      "title": "Clever Chapter Title 32",
      "position": 3,
      "updated_at": "2016-10-26T19:31:41.492Z",
      "course_id": 98,
      "author_id": 302,
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
	-H "Authorization: Bearer 51cce9684842a0c37d3213c0202c267f63c8bbe64b8e0ee8c772842d32237891"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 521e34e93f458931053bdf22c8275407e2ff0bbc85845586ec4386e623ea674c
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
	-H "Authorization: Bearer 521e34e93f458931053bdf22c8275407e2ff0bbc85845586ec4386e623ea674c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/142
Content-Type: application/json
Authorization: Bearer 0aeb5424870afdf8099c43ea89bb55454cfef1b29841e1fc451bcd8f2b435cc9
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/142" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aeb5424870afdf8099c43ea89bb55454cfef1b29841e1fc451bcd8f2b435cc9"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer a0e992fc070fc46cb2b96ddd6f05b6023af56517b6eef54392bfea06c77514ad
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
    "creator_id": 411,
    "id": 130,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 137,
    "additional_university_ids": [

    ],
    "topic_id": 140,
    "discipline_id": 140,
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
    "chapters_updated_at": "2016-10-26T19:31:49.619Z",
    "updated_at": "2016-10-26T19:31:50.949Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 72,
        "title": "Clever Chapter Title 51",
        "position": 1,
        "updated_at": "2016-10-26T19:31:50.907Z",
        "course_id": 130,
        "author_id": 411,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T19:31:49.619Z",
        "questions_updated_at": "2016-10-26T19:31:49.619Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 73,
        "title": "Clever Chapter Title 52",
        "position": 2,
        "updated_at": "2016-10-26T19:31:50.942Z",
        "course_id": 130,
        "author_id": 411,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T19:31:49.619Z",
        "questions_updated_at": "2016-10-26T19:31:49.619Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 411,
        "chapter_id": 72,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.755Z",
        "created_at": "2016-10-26T19:31:50.755Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 411,
        "chapter_id": 73,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.820Z",
        "created_at": "2016-10-26T19:31:50.820Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 411,
        "chapter_id": 72,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.791Z",
        "created_at": "2016-10-26T19:31:50.791Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 411,
        "chapter_id": 73,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.862Z",
        "created_at": "2016-10-26T19:31:50.862Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 414,
        "chapter_id": 72,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.898Z",
        "created_at": "2016-10-26T19:31:50.898Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 415,
        "chapter_id": 73,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:50.933Z",
        "created_at": "2016-10-26T19:31:50.933Z",
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
	-H "Authorization: Bearer a0e992fc070fc46cb2b96ddd6f05b6023af56517b6eef54392bfea06c77514ad"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/125
Content-Type: application/json
Authorization: Bearer cb5a81a76c8034f38132aea2320519d172908a347973d343982502b0efb85af0
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
    "creator_id": 398,
    "id": 125,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 132,
    "additional_university_ids": [

    ],
    "topic_id": 135,
    "discipline_id": 135,
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
    "updated_at": "2016-10-26T19:31:47.864Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/125" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb5a81a76c8034f38132aea2320519d172908a347973d343982502b0efb85af0"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 930d47296aa1024d5ad0bcd183925d9f5ce98403ac5b4903dd3d6009cd02f730
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
    "creator_id": 401,
    "id": 127,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 134,
    "additional_university_ids": [

    ],
    "topic_id": 137,
    "discipline_id": 137,
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
    "updated_at": "2016-10-26T19:31:48.117Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 930d47296aa1024d5ad0bcd183925d9f5ce98403ac5b4903dd3d6009cd02f730"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 5c5b0e53766ca6a96d12bdbab9c960d5358dcdae79492bf61d923b5811d9dfe9
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
      "user_id": 620,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:06.498Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 624,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:06.775Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 628,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:07.053Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 632,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:07.333Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 636,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T19:32:07.614Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c5b0e53766ca6a96d12bdbab9c960d5358dcdae79492bf61d923b5811d9dfe9"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 6454730693a10b049468bf2340d38e27236add6d73e83aeb3577e5346a60e72b
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
      "user_id": 615,
      "feedbackable_id": 86,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T19:32:06.185Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6454730693a10b049468bf2340d38e27236add6d73e83aeb3577e5346a60e72b"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer 335dee98d61ca41da0463c778480758b2fccc5b3d59e62a0b48cf50370419115
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 335dee98d61ca41da0463c778480758b2fccc5b3d59e62a0b48cf50370419115"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer 8124130fa17d1f4b9a4fc8a439bf315992787e325f523746bb3270b331d78d97
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
      "id": 474,
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
      "created_at": "2016-10-26T19:31:56.639Z",
      "updated_at": "2016-10-26T19:31:56.639Z"
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
    "created_at": "2016-10-26T19:31:56.707Z",
    "updated_at": "2016-10-26T19:31:56.707Z",
    "course_id": 152,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8124130fa17d1f4b9a4fc8a439bf315992787e325f523746bb3270b331d78d97"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/90/feedbacks
Content-Type: application/json
Authorization: Bearer ff27b88326022c4976c74f99cab724c7bbbec1f5724db8999c3e680610d18b79
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
      "id": 42,
      "user_id": 950,
      "feedbackable_id": 90,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:31.531Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 949,
      "feedbackable_id": 90,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:31.520Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/90/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff27b88326022c4976c74f99cab724c7bbbec1f5724db8999c3e680610d18b79"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 773984ecda0c9025fb068a57edff4cd69c20c8e9364d4d1a0b8b410226e51ebe
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
      "author_id": 730,
      "chapter_id": 137,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:13.893Z",
      "created_at": "2016-10-26T19:32:13.893Z",
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
      "author_id": 733,
      "chapter_id": 138,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:14.018Z",
      "created_at": "2016-10-26T19:32:14.018Z",
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
      "author_id": 736,
      "chapter_id": 139,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:14.142Z",
      "created_at": "2016-10-26T19:32:14.142Z",
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
      "author_id": 739,
      "chapter_id": 140,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:14.269Z",
      "created_at": "2016-10-26T19:32:14.269Z",
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
      "author_id": 742,
      "chapter_id": 141,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:14.392Z",
      "created_at": "2016-10-26T19:32:14.392Z",
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
	-H "Authorization: Bearer 773984ecda0c9025fb068a57edff4cd69c20c8e9364d4d1a0b8b410226e51ebe"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4a6138deecbe85519a7e7d68d28bb756aba1e832e329a0ce078e0cba70fcd599
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 758,
      "chapter_id": 146,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:15.067Z",
      "created_at": "2016-10-26T19:32:15.067Z",
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
	-H "Authorization: Bearer 4a6138deecbe85519a7e7d68d28bb756aba1e832e329a0ce078e0cba70fcd599"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/republish
Content-Type: application/json
Authorization: Bearer 6ec1370e4be3c9d59b413016692ec8215898b065ce811ed7836d317f031b3f47
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ec1370e4be3c9d59b413016692ec8215898b065ce811ed7836d317f031b3f47"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/69/feedbacks
Content-Type: application/json
Authorization: Bearer befacae77cf5f79fbeaede244c494d12916c954e5c09ba87026dde7a43915a0d
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
      "id": 5,
      "user_id": 500,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:31:58.424Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 499,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:31:58.414Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/69/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer befacae77cf5f79fbeaede244c494d12916c954e5c09ba87026dde7a43915a0d"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 740e52cf8dff1aa81a128feb3539a51a62480183610788bee61a642a681c9fa6
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
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 907,
      "chapter_id": 177,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:27.281Z",
      "created_at": "2016-10-26T19:32:27.163Z",
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
          "id": 250,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 251,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 898,
      "chapter_id": 174,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:26.477Z",
      "created_at": "2016-10-26T19:32:26.367Z",
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
          "id": 244,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 245,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 901,
      "chapter_id": 175,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:26.738Z",
      "created_at": "2016-10-26T19:32:26.626Z",
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
          "id": 246,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 247,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 904,
      "chapter_id": 176,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:27.007Z",
      "created_at": "2016-10-26T19:32:26.892Z",
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
    },
    {
      "id": 125,
      "obfuscated_id": "K6zw0Yc6Me8",
      "author_id": 910,
      "chapter_id": 178,
      "position": 116,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:27.552Z",
      "created_at": "2016-10-26T19:32:27.438Z",
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
          "id": 252,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 253,
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
	-H "Authorization: Bearer 740e52cf8dff1aa81a128feb3539a51a62480183610788bee61a642a681c9fa6"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer a589b9c0b577517ab905d85c4c1370892faf6d9a98cf72e62d1435cf360ec9ec
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
      "id": 120,
      "obfuscated_id": "vEr9LtFjURM",
      "author_id": 894,
      "chapter_id": 173,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:32:26.170Z",
      "created_at": "2016-10-26T19:32:26.058Z",
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
          "id": 242,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 243,
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
	-H "Authorization: Bearer a589b9c0b577517ab905d85c4c1370892faf6d9a98cf72e62d1435cf360ec9ec"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/111/republish
Content-Type: application/json
Authorization: Bearer 704f1f3a59fe72df3caa55b5fdf229427f32bfb74ebbe78a1dc5064f118d009a
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
	-H "Authorization: Bearer 704f1f3a59fe72df3caa55b5fdf229427f32bfb74ebbe78a1dc5064f118d009a"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 54d5d7a13c12f1b074556807e7417dc3d142a7d3d4ca99303acb3a932d7624d9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":279,"published":false}}
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
    "creator_id": 824,
    "id": 267,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 252,
    "additional_university_ids": [

    ],
    "topic_id": 279,
    "discipline_id": 280,
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
    "updated_at": "2016-10-26T19:32:19.878Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":279,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54d5d7a13c12f1b074556807e7417dc3d142a7d3d4ca99303acb3a932d7624d9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 138872faa3e570c79b6cd1532e0ed44b578fb84ee4daf0ee7ea0203e4687606b
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
      "creator_id": 797,
      "id": 243,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 255,
      "discipline_id": 256,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 181",
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
      "updated_at": "2016-10-26T19:32:17.516Z",
      "shortname": "fu-course-181"
    },
    {
      "creator_id": 797,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 182",
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
      "updated_at": "2016-10-26T19:32:17.554Z",
      "shortname": "fu-course-182"
    },
    {
      "creator_id": 798,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-183",
      "html_url": "https://goskive.com/course/fu-course-183",
      "slug": "fu-course-183",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 257,
      "discipline_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 183",
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
      "updated_at": "2016-10-26T19:32:17.598Z",
      "shortname": "fu-course-183"
    },
    {
      "creator_id": 798,
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-184",
      "html_url": "https://goskive.com/course/fu-course-184",
      "slug": "fu-course-184",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 258,
      "discipline_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 184",
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
      "chapters_updated_at": "2016-10-26T19:32:17.872Z",
      "updated_at": "2016-10-26T19:32:17.878Z",
      "shortname": "fu-course-184"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 138872faa3e570c79b6cd1532e0ed44b578fb84ee4daf0ee7ea0203e4687606b"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a717af13f07a0a76b25e2f63b910f13782cade9c3031622f7135e2dea608e676
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
      "creator_id": 804,
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-185",
      "html_url": "https://goskive.com/course/fu-course-185",
      "slug": "fu-course-185",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 259,
      "discipline_id": 260,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
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
      "updated_at": "2016-10-26T19:32:18.069Z",
      "shortname": "fu-course-185"
    },
    {
      "creator_id": 804,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-186",
      "html_url": "https://goskive.com/course/fu-course-186",
      "slug": "fu-course-186",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 260,
      "discipline_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 186",
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
      "updated_at": "2016-10-26T19:32:18.106Z",
      "shortname": "fu-course-186"
    },
    {
      "creator_id": 805,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-187",
      "html_url": "https://goskive.com/course/fu-course-187",
      "slug": "fu-course-187",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 261,
      "discipline_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 187",
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
      "updated_at": "2016-10-26T19:32:18.151Z",
      "shortname": "fu-course-187"
    },
    {
      "creator_id": 805,
      "id": 250,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-188",
      "html_url": "https://goskive.com/course/fu-course-188",
      "slug": "fu-course-188",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 262,
      "discipline_id": 263,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 188",
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
      "updated_at": "2016-10-26T19:32:18.187Z",
      "shortname": "fu-course-188"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a717af13f07a0a76b25e2f63b910f13782cade9c3031622f7135e2dea608e676"
```
