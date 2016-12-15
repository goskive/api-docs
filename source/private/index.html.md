---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Chapters

## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/29
Content-Type: application/json
Authorization: Bearer d813a610fb4b38f3fa5cc2a62f63703b4360c2fd34f01ad4962d79b3d87ae36a
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/29" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d813a610fb4b38f3fa5cc2a62f63703b4360c2fd34f01ad4962d79b3d87ae36a"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/36
Content-Type: application/json
Authorization: Bearer 667300824496ecc22800abf10270474d30afc1bc14c503474cac2170d026ada1
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
    "id": 36,
    "updated_at": "2016-12-15T13:32:20.837Z",
    "course_id": 58,
    "author_id": 211,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-15T13:32:20.270Z",
    "questions_updated_at": "2016-12-15T13:32:20.270Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 214,
        "chapter_id": 36,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:20.773Z",
        "created_at": "2016-12-15T13:32:20.773Z",
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
        "author_id": 215,
        "chapter_id": 36,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:20.816Z",
        "created_at": "2016-12-15T13:32:20.816Z",
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
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 212,
        "chapter_id": 36,
        "position": 20,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:20.529Z",
        "created_at": "2016-12-15T13:32:20.439Z",
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
            "id": 39,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 40,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 213,
        "chapter_id": 36,
        "position": 21,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:20.702Z",
        "created_at": "2016-12-15T13:32:20.603Z",
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
            "id": 41,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 42,
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
curl "api.goskive.com/v2/chapters/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 667300824496ecc22800abf10270474d30afc1bc14c503474cac2170d026ada1"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/34
Content-Type: application/json
Authorization: Bearer ffa098141e5a8654be13c45dec6c37dc27bc6c4c558317db014231de0dbd4e3c
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
    "id": 34,
    "updated_at": "2016-12-15T13:32:20.007Z",
    "course_id": 56,
    "author_id": 206,
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
curl "api.goskive.com/v2/chapters/34" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffa098141e5a8654be13c45dec6c37dc27bc6c4c558317db014231de0dbd4e3c"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/17
Content-Type: application/json
Authorization: Bearer d3d307006f50dd658b61ade44a231f1b82ed354a3843a6016114b553c282d530
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3d307006f50dd658b61ade44a231f1b82ed354a3843a6016114b553c282d530"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 6e91b881e7972fffb733eb67109f9ea2fa506e38c6e191655a78bfe877d1522a
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
      "author_id": 615,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:00.935Z",
      "status": "published",
      "subject_id": 167,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 617,
      "reply_to_id": 21,
      "created_at": "2016-12-15T13:33:01.075Z",
      "status": "published",
      "subject_id": 168,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 619,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:01.208Z",
      "status": "published",
      "subject_id": 169,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 621,
      "reply_to_id": 23,
      "created_at": "2016-12-15T13:33:01.344Z",
      "status": "published",
      "subject_id": 170,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 623,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:01.509Z",
      "status": "reported",
      "subject_id": 171,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 625,
      "reply_to_id": 25,
      "created_at": "2016-12-15T13:33:01.675Z",
      "status": "published",
      "subject_id": 172,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 627,
      "reply_to_id": 25,
      "created_at": "2016-12-15T13:33:01.816Z",
      "status": "published",
      "subject_id": 173,
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
	-H "Authorization: Bearer 6e91b881e7972fffb733eb67109f9ea2fa506e38c6e191655a78bfe877d1522a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5fecad780e2a1d2a1f6404e12638226de49c0ee508fbd0e602dcbae957dbd7d6
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
      "author_id": 630,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:02.019Z",
      "status": "published",
      "subject_id": 174,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 632,
      "reply_to_id": 28,
      "created_at": "2016-12-15T13:33:02.149Z",
      "status": "published",
      "subject_id": 175,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 634,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:02.281Z",
      "status": "published",
      "subject_id": 176,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 636,
      "reply_to_id": 30,
      "created_at": "2016-12-15T13:33:02.421Z",
      "status": "published",
      "subject_id": 177,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 638,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:02.560Z",
      "status": "reported",
      "subject_id": 178,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 640,
      "reply_to_id": 32,
      "created_at": "2016-12-15T13:33:02.695Z",
      "status": "published",
      "subject_id": 179,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 642,
      "reply_to_id": 32,
      "created_at": "2016-12-15T13:33:02.836Z",
      "status": "published",
      "subject_id": 180,
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
	-H "Authorization: Bearer 5fecad780e2a1d2a1f6404e12638226de49c0ee508fbd0e602dcbae957dbd7d6"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer edd379b697d5aeca8ab75280662b3cc05b40d66680080abcba8f1b98e217d2bb
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
      "id": 50,
      "author_id": 677,
      "reply_to_id": 49,
      "created_at": "2016-12-15T13:33:05.244Z",
      "status": "published",
      "subject_id": 196,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 681,
      "reply_to_id": 51,
      "created_at": "2016-12-15T13:33:05.518Z",
      "status": "published",
      "subject_id": 198,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 54,
      "author_id": 685,
      "reply_to_id": 53,
      "created_at": "2016-12-15T13:33:05.791Z",
      "status": "published",
      "subject_id": 200,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 687,
      "reply_to_id": 53,
      "created_at": "2016-12-15T13:33:05.928Z",
      "status": "published",
      "subject_id": 201,
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
	-H "Authorization: Bearer edd379b697d5aeca8ab75280662b3cc05b40d66680080abcba8f1b98e217d2bb"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 218176a498a95a1ce62e48866f5fb0e8e61a4911bc54d61aa8bff49570c67da2
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
      "id": 46,
      "author_id": 668,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:33:04.618Z",
      "status": "reported",
      "subject_id": 192,
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
	-H "Authorization: Bearer 218176a498a95a1ce62e48866f5fb0e8e61a4911bc54d61aa8bff49570c67da2"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/19/republish
Content-Type: application/json
Authorization: Bearer ea2fedf9afaef28592928046ba1f54a1b18d278928853bc058d35cca04aaad95
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/19/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea2fedf9afaef28592928046ba1f54a1b18d278928853bc058d35cca04aaad95"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/230/chapters
Content-Type: application/json
Authorization: Bearer aaa0fcfc8e54ea10557eaf6b33ae449710bf33b1653f273204a481684958a283
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
    "id": 143,
    "updated_at": "2016-12-15T13:33:16.186Z",
    "course_id": 230,
    "author_id": 781,
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
curl "api.goskive.com/v2/courses/230/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aaa0fcfc8e54ea10557eaf6b33ae449710bf33b1653f273204a481684958a283"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 90bd80d9ee6cdc4f2a122e83f0b3b4db4e8127fbf4a4e3a081b3de31c1471ab6
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
    "id": 144,
    "updated_at": "2016-12-15T13:33:16.545Z",
    "course_id": 232,
    "author_id": 785,
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
	-H "Authorization: Bearer 90bd80d9ee6cdc4f2a122e83f0b3b4db4e8127fbf4a4e3a081b3de31c1471ab6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b59a19cb3ebb478d804acb45b890c2d04a748c259a9e1bfa06003da00ae34a50
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
      "id": 161,
      "updated_at": "2016-12-15T13:33:19.177Z",
      "course_id": 242,
      "author_id": 821,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 146",
      "position": 1
    },
    {
      "id": 162,
      "updated_at": "2016-12-15T13:33:19.204Z",
      "course_id": 242,
      "author_id": 822,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 147",
      "position": 2
    },
    {
      "id": 163,
      "updated_at": "2016-12-15T13:33:19.428Z",
      "course_id": 242,
      "author_id": 823,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-15T13:33:19.049Z",
      "questions_updated_at": "2016-12-15T13:33:19.049Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 148",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b59a19cb3ebb478d804acb45b890c2d04a748c259a9e1bfa06003da00ae34a50"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 71dbc600a289f0eb8640f4d32ed9f2b7ba178ea292bddbeedeb1cc6a6b154c8e
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
      "id": 164,
      "updated_at": "2016-12-15T13:33:19.797Z",
      "course_id": 244,
      "author_id": 830,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 149",
      "position": 1
    },
    {
      "id": 165,
      "updated_at": "2016-12-15T13:33:19.823Z",
      "course_id": 244,
      "author_id": 831,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 150",
      "position": 2
    },
    {
      "id": 166,
      "updated_at": "2016-12-15T13:33:19.850Z",
      "course_id": 244,
      "author_id": 832,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 151",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71dbc600a289f0eb8640f4d32ed9f2b7ba178ea292bddbeedeb1cc6a6b154c8e"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1ff8c5717b39321fb49d21f26a3cc1f042fbc6624bec632b712b2cc09f33fa5e
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
	-H "Authorization: Bearer 1ff8c5717b39321fb49d21f26a3cc1f042fbc6624bec632b712b2cc09f33fa5e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/158
Content-Type: application/json
Authorization: Bearer 34070852be4575c843d75ca3f7d6cad22958f97d10a9a79f94e1217586eccf4d
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/158" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34070852be4575c843d75ca3f7d6cad22958f97d10a9a79f94e1217586eccf4d"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 79fb61df35a9356635e205968109b5546d4aa17c2a83fafea16ff57ded48120f
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
    "creator_id": 535,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 147,
    "additional_university_ids": [

    ],
    "discipline_id": 151,
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
    "chapters_updated_at": "2016-12-15T13:32:48.640Z",
    "updated_at": "2016-12-15T13:32:50.212Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 535,
        "chapter_id": 105,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:49.940Z",
        "created_at": "2016-12-15T13:32:49.940Z",
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
        "author_id": 535,
        "chapter_id": 106,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:50.034Z",
        "created_at": "2016-12-15T13:32:50.034Z",
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
        "author_id": 535,
        "chapter_id": 105,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:49.993Z",
        "created_at": "2016-12-15T13:32:49.993Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 535,
        "chapter_id": 106,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:50.087Z",
        "created_at": "2016-12-15T13:32:50.087Z",
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
        "author_id": 538,
        "chapter_id": 105,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:50.137Z",
        "created_at": "2016-12-15T13:32:50.137Z",
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
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 539,
        "chapter_id": 106,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:50.186Z",
        "created_at": "2016-12-15T13:32:50.186Z",
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
        "id": 105,
        "updated_at": "2016-12-15T13:32:50.150Z",
        "course_id": 141,
        "author_id": 535,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T13:32:48.640Z",
        "questions_updated_at": "2016-12-15T13:32:48.640Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 96",
        "position": 1
      },
      {
        "id": 106,
        "updated_at": "2016-12-15T13:32:50.199Z",
        "course_id": 141,
        "author_id": 535,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T13:32:48.640Z",
        "questions_updated_at": "2016-12-15T13:32:48.640Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 97",
        "position": 2
      }
    ],
    "topic_id": 150,
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
	-H "Authorization: Bearer 79fb61df35a9356635e205968109b5546d4aa17c2a83fafea16ff57ded48120f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/149
Content-Type: application/json
Authorization: Bearer f79bab9e592badb5563d021a092336281c6f64eeaf211303af25b901c02c054e
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
    "creator_id": 561,
    "id": 149,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 155,
    "additional_university_ids": [

    ],
    "discipline_id": 159,
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
    "updated_at": "2016-12-15T13:32:54.881Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 158,
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
curl "api.goskive.com/v2/courses/149" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f79bab9e592badb5563d021a092336281c6f64eeaf211303af25b901c02c054e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 14a8c75aa1c4786c103bd0a344528a914b0c29e9a996af308e84463837ea1df9
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
    "creator_id": 559,
    "id": 148,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 154,
    "additional_university_ids": [

    ],
    "discipline_id": 158,
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
    "updated_at": "2016-12-15T13:32:54.670Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 157,
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
	-H "Authorization: Bearer 14a8c75aa1c4786c103bd0a344528a914b0c29e9a996af308e84463837ea1df9"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 9e08953f47b8a2e373eac6f9488e6b0d461f9f8ecf8cf205a0e121e96e2d7418
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
      "id": 11,
      "user_id": 240,
      "feedbackable_id": 24,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:22.709Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 244,
      "feedbackable_id": 25,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:23.045Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 248,
      "feedbackable_id": 26,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:23.379Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 252,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:23.712Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 256,
      "feedbackable_id": 28,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T13:32:24.054Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e08953f47b8a2e373eac6f9488e6b0d461f9f8ecf8cf205a0e121e96e2d7418"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer e461a3f4ede93bd90b10a74c03d7f86d6224fa5f050110fcc3569e24b42f0831
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
      "id": 29,
      "user_id": 314,
      "feedbackable_id": 42,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T13:32:28.858Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e461a3f4ede93bd90b10a74c03d7f86d6224fa5f050110fcc3569e24b42f0831"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer 8b11ba8f3d15cc376d9b1fe028860f08dd25ccdd2caf6b4c09b8146f03378504
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b11ba8f3d15cc376d9b1fe028860f08dd25ccdd2caf6b4c09b8146f03378504"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/22/metadata
Content-Type: application/json
Authorization: Bearer c4fe6edd6c5e71d7bc04b396a561a720add9e8a06192ce11c569d1f1e7c821c9
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
    "id": 22,
    "uploader": {
      "id": 495,
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
      "created_at": "2016-12-15T13:32:42.662Z",
      "updated_at": "2016-12-15T13:32:42.662Z"
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
    "created_at": "2016-12-15T13:32:42.790Z",
    "updated_at": "2016-12-15T13:32:42.790Z",
    "course_id": 130,
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
curl "api.goskive.com/v2/files/22/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4fe6edd6c5e71d7bc04b396a561a720add9e8a06192ce11c569d1f1e7c821c9"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/11/feedbacks
Content-Type: application/json
Authorization: Bearer 6fc68290984caf4d409f2ae84c4063ff1f28809d434e3ddbd04e1a9f287fe729
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
      "id": 4,
      "user_id": 129,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:12.545Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 128,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:12.533Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/11/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fc68290984caf4d409f2ae84c4063ff1f28809d434e3ddbd04e1a9f287fe729"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 08eb47d1d158e681434c23a6f58dafdd6a2221b47cbe83c1968cb3d4640d4ea6
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
      "author_id": 419,
      "chapter_id": 85,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:36.926Z",
      "created_at": "2016-12-15T13:32:36.926Z",
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
      "author_id": 422,
      "chapter_id": 86,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:37.124Z",
      "created_at": "2016-12-15T13:32:37.124Z",
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
      "author_id": 425,
      "chapter_id": 87,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:37.318Z",
      "created_at": "2016-12-15T13:32:37.318Z",
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
      "author_id": 428,
      "chapter_id": 88,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:37.515Z",
      "created_at": "2016-12-15T13:32:37.515Z",
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
      "author_id": 431,
      "chapter_id": 89,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:37.714Z",
      "created_at": "2016-12-15T13:32:37.714Z",
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
	-H "Authorization: Bearer 08eb47d1d158e681434c23a6f58dafdd6a2221b47cbe83c1968cb3d4640d4ea6"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 1cf0ede6bfacdebb4df633fc67cb94ac2741bf416f75c3fb43d2cc09ebf8e276
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
      "id": 46,
      "obfuscated_id": "urkHiAaH08E",
      "author_id": 399,
      "chapter_id": 79,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:32:35.624Z",
      "created_at": "2016-12-15T13:32:35.624Z",
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
	-H "Authorization: Bearer 1cf0ede6bfacdebb4df633fc67cb94ac2741bf416f75c3fb43d2cc09ebf8e276"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/34/republish
Content-Type: application/json
Authorization: Bearer 4bcab39169b3c4632cf82c5de66ac3d4a5b55da6c589ab078354d97197cd7abe
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4bcab39169b3c4632cf82c5de66ac3d4a5b55da6c589ab078354d97197cd7abe"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/116/feedbacks
Content-Type: application/json
Authorization: Bearer d47831df43b0b39bc40f2cd2b125a5273a6eb3e05b3f5911d12991fbd1d6fd94
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
      "user_id": 896,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:33:26.408Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 895,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:33:26.396Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/116/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d47831df43b0b39bc40f2cd2b125a5273a6eb3e05b3f5911d12991fbd1d6fd94"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 28a305dcf0444f3a0986e524bbd1243e9c4dd23510d15646a2af5d9aab110cd1
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
      "author_id": 748,
      "chapter_id": 132,
      "position": 87,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:12.119Z",
      "created_at": "2016-12-15T13:33:12.034Z",
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
          "id": 181,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 182,
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
      "author_id": 751,
      "chapter_id": 133,
      "position": 88,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:12.421Z",
      "created_at": "2016-12-15T13:33:12.332Z",
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
          "id": 183,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 184,
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
      "author_id": 754,
      "chapter_id": 134,
      "position": 89,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:12.723Z",
      "created_at": "2016-12-15T13:33:12.633Z",
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
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 757,
      "chapter_id": 135,
      "position": 90,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:13.042Z",
      "created_at": "2016-12-15T13:33:12.949Z",
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
      "id": 95,
      "obfuscated_id": "uTOhBSQK4CI",
      "author_id": 760,
      "chapter_id": 136,
      "position": 91,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:13.354Z",
      "created_at": "2016-12-15T13:33:13.269Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28a305dcf0444f3a0986e524bbd1243e9c4dd23510d15646a2af5d9aab110cd1"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer b849fb716e94dc8b61deafa027bac0d6700a47d0fc8e3bddd4365a53244d071e
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
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 744,
      "chapter_id": 131,
      "position": 86,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:11.769Z",
      "created_at": "2016-12-15T13:33:11.689Z",
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
          "id": 179,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 180,
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
	-H "Authorization: Bearer b849fb716e94dc8b61deafa027bac0d6700a47d0fc8e3bddd4365a53244d071e"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/99/republish
Content-Type: application/json
Authorization: Bearer e75527e8238a0701305be836342ee6e9e9a4eab9d27e0fbc1fda53253a6ad5f5
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/99/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e75527e8238a0701305be836342ee6e9e9a4eab9d27e0fbc1fda53253a6ad5f5"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b4432d7b6a27c08742ed715dfaf37a45b3290e67ec37d2e0207d3b99fc3a68c2
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":289,"published":false}}
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
    "creator_id": 944,
    "id": 277,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 284,
    "additional_university_ids": [

    ],
    "discipline_id": 290,
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
    "updated_at": "2016-12-15T13:33:32.668Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 289,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":289,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4432d7b6a27c08742ed715dfaf37a45b3290e67ec37d2e0207d3b99fc3a68c2"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 14bf64f28a4e45fdcc9c7965f96db7c9a9505bbca64ea2715ca2886265934938
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
      "creator_id": 962,
      "id": 293,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-221",
      "html_url": "https://goskive.com/course/fu-course-221",
      "slug": "fu-course-221",
      "university_id": 293,
      "additional_university_ids": [

      ],
      "discipline_id": 306,
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
      "updated_at": "2016-12-15T13:33:34.939Z",
      "shortname": "fu-course-221",
      "topic_id": 305,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 221",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 962,
      "id": 294,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-222",
      "html_url": "https://goskive.com/course/fu-course-222",
      "slug": "fu-course-222",
      "university_id": 293,
      "additional_university_ids": [

      ],
      "discipline_id": 307,
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
      "updated_at": "2016-12-15T13:33:34.975Z",
      "shortname": "fu-course-222",
      "topic_id": 306,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 222",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 963,
      "id": 295,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-223",
      "html_url": "https://goskive.com/course/fu-course-223",
      "slug": "fu-course-223",
      "university_id": 293,
      "additional_university_ids": [

      ],
      "discipline_id": 308,
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
      "updated_at": "2016-12-15T13:33:35.016Z",
      "shortname": "fu-course-223",
      "topic_id": 307,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 223",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 963,
      "id": 296,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-224",
      "html_url": "https://goskive.com/course/fu-course-224",
      "slug": "fu-course-224",
      "university_id": 293,
      "additional_university_ids": [

      ],
      "discipline_id": 309,
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
      "chapters_updated_at": "2016-12-15T13:33:34.802Z",
      "updated_at": "2016-12-15T13:33:35.283Z",
      "shortname": "fu-course-224",
      "topic_id": 308,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 224",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14bf64f28a4e45fdcc9c7965f96db7c9a9505bbca64ea2715ca2886265934938"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0d6f163a494209d9c0b371997f4c9cb285d5548806b7dc35f07648fa6315f41d
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
      "creator_id": 968,
      "id": 297,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-225",
      "html_url": "https://goskive.com/course/fu-course-225",
      "slug": "fu-course-225",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 310,
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
      "updated_at": "2016-12-15T13:33:35.503Z",
      "shortname": "fu-course-225",
      "topic_id": 309,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 225",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 968,
      "id": 298,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-226",
      "html_url": "https://goskive.com/course/fu-course-226",
      "slug": "fu-course-226",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 311,
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
      "updated_at": "2016-12-15T13:33:35.538Z",
      "shortname": "fu-course-226",
      "topic_id": 310,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 226",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 969,
      "id": 299,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-227",
      "html_url": "https://goskive.com/course/fu-course-227",
      "slug": "fu-course-227",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 312,
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
      "updated_at": "2016-12-15T13:33:35.583Z",
      "shortname": "fu-course-227",
      "topic_id": 311,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 227",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 969,
      "id": 300,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-228",
      "html_url": "https://goskive.com/course/fu-course-228",
      "slug": "fu-course-228",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 313,
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
      "updated_at": "2016-12-15T13:33:35.620Z",
      "shortname": "fu-course-228",
      "topic_id": 312,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 228",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d6f163a494209d9c0b371997f4c9cb285d5548806b7dc35f07648fa6315f41d"
```
