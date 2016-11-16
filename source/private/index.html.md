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
DELETE /v2/chapters/99
Content-Type: application/json
Authorization: Bearer 5a83f57e7c6c6a48acbaed01e2fe66a6ef0b6b3f47e279963290a04ec11604d5
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/99" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a83f57e7c6c6a48acbaed01e2fe66a6ef0b6b3f47e279963290a04ec11604d5"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/103
Content-Type: application/json
Authorization: Bearer bf2822ed7e5826f69275f1ca9a5366dc4f22e0cdcc9b774267faa7c85e91291e
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
    "id": 103,
    "updated_at": "2016-11-16T17:41:02.526Z",
    "course_id": 116,
    "author_id": 438,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-16T17:41:01.998Z",
    "questions_updated_at": "2016-11-16T17:41:01.998Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 441,
        "chapter_id": 103,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:02.472Z",
        "created_at": "2016-11-16T17:41:02.472Z",
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
        "author_id": 442,
        "chapter_id": 103,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:02.508Z",
        "created_at": "2016-11-16T17:41:02.508Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 439,
        "chapter_id": 103,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:02.211Z",
        "created_at": "2016-11-16T17:41:02.101Z",
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
            "id": 142,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 143,
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
        "author_id": 440,
        "chapter_id": 103,
        "position": 63,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:02.403Z",
        "created_at": "2016-11-16T17:41:02.283Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/103" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf2822ed7e5826f69275f1ca9a5366dc4f22e0cdcc9b774267faa7c85e91291e"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/105
Content-Type: application/json
Authorization: Bearer f0a65485406db7fd216e02a1aa68b3331fd76df530d6cb74d2e02d0d093b1433
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
    "id": 105,
    "updated_at": "2016-11-16T17:41:02.921Z",
    "course_id": 118,
    "author_id": 447,
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
curl "api.goskive.com/v2/chapters/105" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0a65485406db7fd216e02a1aa68b3331fd76df530d6cb74d2e02d0d093b1433"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/46
Content-Type: application/json
Authorization: Bearer 0c746ec3a8d3124163c87825c19e33386cdde5368980dfdb3bab1ef6c0a75297
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c746ec3a8d3124163c87825c19e33386cdde5368980dfdb3bab1ef6c0a75297"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer bbcef2edd6a8d179322b40928988946275f80526e2f75eb0e0cb510ee5989ce4
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
      "id": 18,
      "author_id": 640,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:22.564Z",
      "status": "published",
      "subject_id": 206,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 642,
      "reply_to_id": 18,
      "created_at": "2016-11-16T17:41:22.648Z",
      "status": "published",
      "subject_id": 207,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 644,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:22.735Z",
      "status": "published",
      "subject_id": 208,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 646,
      "reply_to_id": 20,
      "created_at": "2016-11-16T17:41:22.822Z",
      "status": "published",
      "subject_id": 209,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 648,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:22.905Z",
      "status": "reported",
      "subject_id": 210,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 650,
      "reply_to_id": 22,
      "created_at": "2016-11-16T17:41:22.989Z",
      "status": "published",
      "subject_id": 211,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 652,
      "reply_to_id": 22,
      "created_at": "2016-11-16T17:41:23.074Z",
      "status": "published",
      "subject_id": 212,
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
	-H "Authorization: Bearer bbcef2edd6a8d179322b40928988946275f80526e2f75eb0e0cb510ee5989ce4"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5f56268f82d564fd443c7002bdb04fb89171521e5a37d20846edaca1ffed1c3c
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
      "id": 25,
      "author_id": 655,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:23.245Z",
      "status": "published",
      "subject_id": 213,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 657,
      "reply_to_id": 25,
      "created_at": "2016-11-16T17:41:23.330Z",
      "status": "published",
      "subject_id": 214,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 659,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:23.415Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 661,
      "reply_to_id": 27,
      "created_at": "2016-11-16T17:41:23.498Z",
      "status": "published",
      "subject_id": 216,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 663,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:23.583Z",
      "status": "reported",
      "subject_id": 217,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 665,
      "reply_to_id": 29,
      "created_at": "2016-11-16T17:41:23.667Z",
      "status": "published",
      "subject_id": 218,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 667,
      "reply_to_id": 29,
      "created_at": "2016-11-16T17:41:23.752Z",
      "status": "published",
      "subject_id": 219,
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
	-H "Authorization: Bearer 5f56268f82d564fd443c7002bdb04fb89171521e5a37d20846edaca1ffed1c3c"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 4290fd620ca3b0ef2731a7e0f376eaf94afb3f939942dea1d61aba4eeefb5086
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
      "id": 33,
      "author_id": 672,
      "reply_to_id": 32,
      "created_at": "2016-11-16T17:41:23.977Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 676,
      "reply_to_id": 34,
      "created_at": "2016-11-16T17:41:24.146Z",
      "status": "published",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 680,
      "reply_to_id": 36,
      "created_at": "2016-11-16T17:41:24.317Z",
      "status": "published",
      "subject_id": 225,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 682,
      "reply_to_id": 36,
      "created_at": "2016-11-16T17:41:24.401Z",
      "status": "published",
      "subject_id": 226,
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
	-H "Authorization: Bearer 4290fd620ca3b0ef2731a7e0f376eaf94afb3f939942dea1d61aba4eeefb5086"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer bfb41055aebab585e00bdaee66f57761e5ff993f64792a108722ef6d7e595bd0
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
      "id": 15,
      "author_id": 633,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:22.267Z",
      "status": "reported",
      "subject_id": 203,
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
	-H "Authorization: Bearer bfb41055aebab585e00bdaee66f57761e5ff993f64792a108722ef6d7e595bd0"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/8/republish
Content-Type: application/json
Authorization: Bearer 155bf8375f3b9a1ba13a2a0e8d5ae090779e2e00f8825ec3c7b489959b96d791
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
	-H "Authorization: Bearer 155bf8375f3b9a1ba13a2a0e8d5ae090779e2e00f8825ec3c7b489959b96d791"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1db58ba6e9fd91d6f2be51c3149c7b1f14d332d8476723a7b3397482ff65f580
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
    "updated_at": "2016-11-16T17:40:53.894Z",
    "course_id": 80,
    "author_id": 321,
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
	-H "Authorization: Bearer 1db58ba6e9fd91d6f2be51c3149c7b1f14d332d8476723a7b3397482ff65f580"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/82/chapters
Content-Type: application/json
Authorization: Bearer 10b752dd43390c423369367b426541f646f9b55ae1270252484ae1d1e27fb13d
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
    "id": 73,
    "updated_at": "2016-11-16T17:40:54.270Z",
    "course_id": 82,
    "author_id": 325,
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
curl "api.goskive.com/v2/courses/82/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10b752dd43390c423369367b426541f646f9b55ae1270252484ae1d1e27fb13d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2c5b8e8da3b6e7326413616a11314ecea1f63d3a8a1c9bd830e133bce8d464ef
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
      "id": 89,
      "updated_at": "2016-11-16T17:40:56.476Z",
      "course_id": 91,
      "author_id": 359,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 86",
      "position": 1
    },
    {
      "id": 90,
      "updated_at": "2016-11-16T17:40:56.499Z",
      "course_id": 91,
      "author_id": 360,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 87",
      "position": 2
    },
    {
      "id": 91,
      "updated_at": "2016-11-16T17:40:56.744Z",
      "course_id": 91,
      "author_id": 361,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-16T17:40:56.394Z",
      "questions_updated_at": "2016-11-16T17:40:56.394Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 88",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c5b8e8da3b6e7326413616a11314ecea1f63d3a8a1c9bd830e133bce8d464ef"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e1565af96b8b442a7ffb45567a7f9b752f359c9b7d481113ac1e0fcf5e5c4ce7
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
      "id": 92,
      "updated_at": "2016-11-16T17:40:56.998Z",
      "course_id": 93,
      "author_id": 368,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 89",
      "position": 1
    },
    {
      "id": 93,
      "updated_at": "2016-11-16T17:40:57.021Z",
      "course_id": 93,
      "author_id": 369,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 90",
      "position": 2
    },
    {
      "id": 94,
      "updated_at": "2016-11-16T17:40:57.043Z",
      "course_id": 93,
      "author_id": 370,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 91",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1565af96b8b442a7ffb45567a7f9b752f359c9b7d481113ac1e0fcf5e5c4ce7"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/138
Content-Type: application/json
Authorization: Bearer d093fe691ded151ba8621ccd2f4f73db4b0511202d07c26d5c4033e361003c7d
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/138" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d093fe691ded151ba8621ccd2f4f73db4b0511202d07c26d5c4033e361003c7d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e0ff17f6b54d11a99d1cd4e076e441a210aea4b633e72b26e10ca6b09899bfdb
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
	-H "Authorization: Bearer e0ff17f6b54d11a99d1cd4e076e441a210aea4b633e72b26e10ca6b09899bfdb"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 5e0b2d76cec198ad3a75fefd497dc2fe892ca06a9a9a5560879b342c378bcb97
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
    "creator_id": 556,
    "id": 151,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 152,
    "additional_university_ids": [

    ],
    "discipline_id": 164,
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
    "chapters_updated_at": "2016-11-16T17:41:14.664Z",
    "updated_at": "2016-11-16T17:41:16.207Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 556,
        "chapter_id": 121,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:15.988Z",
        "created_at": "2016-11-16T17:41:15.988Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 556,
        "chapter_id": 122,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:16.064Z",
        "created_at": "2016-11-16T17:41:16.064Z",
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
        "author_id": 556,
        "chapter_id": 121,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:16.030Z",
        "created_at": "2016-11-16T17:41:16.030Z",
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
        "author_id": 556,
        "chapter_id": 122,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:16.106Z",
        "created_at": "2016-11-16T17:41:16.106Z",
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
        "author_id": 559,
        "chapter_id": 121,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:16.147Z",
        "created_at": "2016-11-16T17:41:16.147Z",
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
        "author_id": 560,
        "chapter_id": 122,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:16.188Z",
        "created_at": "2016-11-16T17:41:16.188Z",
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
        "id": 121,
        "updated_at": "2016-11-16T17:41:16.158Z",
        "course_id": 151,
        "author_id": 556,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-16T17:41:14.664Z",
        "questions_updated_at": "2016-11-16T17:41:14.664Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 109",
        "position": 1
      },
      {
        "id": 122,
        "updated_at": "2016-11-16T17:41:16.199Z",
        "course_id": 151,
        "author_id": 556,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-16T17:41:14.664Z",
        "questions_updated_at": "2016-11-16T17:41:14.664Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 110",
        "position": 2
      }
    ],
    "topic_id": 163,
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
	-H "Authorization: Bearer 5e0b2d76cec198ad3a75fefd497dc2fe892ca06a9a9a5560879b342c378bcb97"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/155
Content-Type: application/json
Authorization: Bearer 0e3a6319aeb5568ec80499f1fff90ad7c2d49e96555eebb739159d3c3c47bcfc
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
    "creator_id": 567,
    "id": 155,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 156,
    "additional_university_ids": [

    ],
    "discipline_id": 168,
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
    "updated_at": "2016-11-16T17:41:16.871Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 167,
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
curl "api.goskive.com/v2/courses/155" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e3a6319aeb5568ec80499f1fff90ad7c2d49e96555eebb739159d3c3c47bcfc"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4d49b147f47981ab4f01ab9de20ad0b1e1773bab2ebb1b4a4170c78980c850dd
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
    "creator_id": 563,
    "id": 153,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 154,
    "additional_university_ids": [

    ],
    "discipline_id": 166,
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
    "updated_at": "2016-11-16T17:41:16.608Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 165,
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
	-H "Authorization: Bearer 4d49b147f47981ab4f01ab9de20ad0b1e1773bab2ebb1b4a4170c78980c850dd"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 065a76ea40a42c8a2f5d027c7cd1575a48598d23f9b7737be95eea864d024234
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
      "id": 9,
      "user_id": 40,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:22.288Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 44,
      "feedbackable_id": 7,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:22.579Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 48,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:22.874Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 52,
      "feedbackable_id": 9,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:23.164Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 56,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-16T17:40:23.464Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 065a76ea40a42c8a2f5d027c7cd1575a48598d23f9b7737be95eea864d024234"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 58f925e6555788ec814555db02ca00b14529423ad46074eb37bad5bb68d74ba0
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
      "id": 8,
      "user_id": 35,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-16T17:40:21.907Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58f925e6555788ec814555db02ca00b14529423ad46074eb37bad5bb68d74ba0"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 11e51bb19c84bf916851ee7663e5075e083944af0b79f1bb1208a06d6183e067
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11e51bb19c84bf916851ee7663e5075e083944af0b79f1bb1208a06d6183e067"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 655b4eaeb755131f83e8dd3ed1f402c8061b4b808871c48164422b6c23e7df45
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
    "id": 8,
    "uploader": {
      "id": 481,
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
      "created_at": "2016-11-16T17:41:06.031Z",
      "updated_at": "2016-11-16T17:41:06.031Z"
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
    "created_at": "2016-11-16T17:41:06.106Z",
    "updated_at": "2016-11-16T17:41:06.106Z",
    "course_id": 125,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 655b4eaeb755131f83e8dd3ed1f402c8061b4b808871c48164422b6c23e7df45"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/60/feedbacks
Content-Type: application/json
Authorization: Bearer 7342f028724026b615cfbbbd11a2f68cc0b8e55c97d221854c93ad58927eaf5d
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
      "id": 41,
      "user_id": 722,
      "feedbackable_id": 60,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:41:26.204Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 721,
      "feedbackable_id": 60,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:41:26.193Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/60/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7342f028724026b615cfbbbd11a2f68cc0b8e55c97d221854c93ad58927eaf5d"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 7f38032c50c297938ceda47cb035c53552e9de8bdce9119dde1c5c7b2899292a
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
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 880,
      "chapter_id": 168,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:39.427Z",
      "created_at": "2016-11-16T17:41:39.427Z",
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
      "author_id": 883,
      "chapter_id": 169,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:39.559Z",
      "created_at": "2016-11-16T17:41:39.559Z",
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
      "author_id": 886,
      "chapter_id": 170,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:39.705Z",
      "created_at": "2016-11-16T17:41:39.705Z",
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
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 889,
      "chapter_id": 171,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:39.840Z",
      "created_at": "2016-11-16T17:41:39.840Z",
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
      "id": 86,
      "obfuscated_id": "7q-2LHZR3Kk",
      "author_id": 892,
      "chapter_id": 172,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:39.973Z",
      "created_at": "2016-11-16T17:41:39.973Z",
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
	-H "Authorization: Bearer 7f38032c50c297938ceda47cb035c53552e9de8bdce9119dde1c5c7b2899292a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 90acef0b5ca9d31535b4496236550899f130bd1da9e21c5ffbf57e80ef451b23
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
      "author_id": 860,
      "chapter_id": 162,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:38.515Z",
      "created_at": "2016-11-16T17:41:38.515Z",
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
	-H "Authorization: Bearer 90acef0b5ca9d31535b4496236550899f130bd1da9e21c5ffbf57e80ef451b23"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/70/republish
Content-Type: application/json
Authorization: Bearer 2309e0a4b5c3152526fd006d83388387bbe3b9a925347f666cdecad6b79e7f31
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/70/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2309e0a4b5c3152526fd006d83388387bbe3b9a925347f666cdecad6b79e7f31"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/45/feedbacks
Content-Type: application/json
Authorization: Bearer 5a451dd838d9b0f4fb0262145a2a4e5a157c97a47d1a943f99b68fd85e81d50b
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
      "id": 30,
      "user_id": 232,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:40.153Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 231,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:40.142Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/45/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a451dd838d9b0f4fb0262145a2a4e5a157c97a47d1a943f99b68fd85e81d50b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 00f1879ad0686673ec4fd8a4074cb99bd844152c9daf795b1731b12dd739bc3f
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
      "id": 38,
      "obfuscated_id": "8_YCqPYFnsI",
      "author_id": 196,
      "chapter_id": 47,
      "position": 33,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:35.063Z",
      "created_at": "2016-11-16T17:40:34.924Z",
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
          "id": 75,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 76,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 187,
      "chapter_id": 44,
      "position": 30,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:34.161Z",
      "created_at": "2016-11-16T17:40:34.027Z",
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
          "id": 69,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 70,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 190,
      "chapter_id": 45,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:34.459Z",
      "created_at": "2016-11-16T17:40:34.325Z",
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
          "id": 71,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 72,
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
      "author_id": 193,
      "chapter_id": 46,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:34.759Z",
      "created_at": "2016-11-16T17:40:34.623Z",
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
          "id": 73,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 74,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 199,
      "chapter_id": 48,
      "position": 34,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:35.361Z",
      "created_at": "2016-11-16T17:40:35.232Z",
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
          "id": 77,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 78,
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
	-H "Authorization: Bearer 00f1879ad0686673ec4fd8a4074cb99bd844152c9daf795b1731b12dd739bc3f"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer f47f8d6d8dae9108c2a77a4cd254b8320162ec9b634169224332dc741b79bb87
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 183,
      "chapter_id": 43,
      "position": 29,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:40:33.821Z",
      "created_at": "2016-11-16T17:40:33.691Z",
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
          "id": 67,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 68,
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
	-H "Authorization: Bearer f47f8d6d8dae9108c2a77a4cd254b8320162ec9b634169224332dc741b79bb87"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/42/republish
Content-Type: application/json
Authorization: Bearer f7e5f57449e9d3b837ba30323ec3f1b8da87a99218c9a89fbea760f03507e59e
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7e5f57449e9d3b837ba30323ec3f1b8da87a99218c9a89fbea760f03507e59e"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a30880d85de3f4899e5545c381b42cd935d4fbe7ffbc8376d84275bebd1ce7cf
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":168,"published":false}}
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
    "creator_id": 569,
    "id": 156,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 157,
    "additional_university_ids": [

    ],
    "discipline_id": 169,
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
    "updated_at": "2016-11-16T17:41:17.031Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 168,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":168,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a30880d85de3f4899e5545c381b42cd935d4fbe7ffbc8376d84275bebd1ce7cf"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 707ffa7d70f1ebaa9dda383abc610049f9b5846414ce180f0a95fb57fbdce289
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
      "creator_id": 590,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-121",
      "html_url": "https://goskive.com/course/fu-course-121",
      "slug": "fu-course-121",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 189,
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
      "updated_at": "2016-11-16T17:41:19.326Z",
      "shortname": "fu-course-121",
      "topic_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 121",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 590,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 190,
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
      "updated_at": "2016-11-16T17:41:19.365Z",
      "shortname": "fu-course-122",
      "topic_id": 189,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 122",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 591,
      "id": 178,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 191,
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
      "updated_at": "2016-11-16T17:41:19.411Z",
      "shortname": "fu-course-123",
      "topic_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 591,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-124",
      "html_url": "https://goskive.com/course/fu-course-124",
      "slug": "fu-course-124",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 192,
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
      "chapters_updated_at": "2016-11-16T17:41:19.269Z",
      "updated_at": "2016-11-16T17:41:19.720Z",
      "shortname": "fu-course-124",
      "topic_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 124",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 707ffa7d70f1ebaa9dda383abc610049f9b5846414ce180f0a95fb57fbdce289"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 41e2240243f5f474612d8000652c60a61f3430fe26f84958729243442e0c9ade
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
      "creator_id": 596,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-125",
      "html_url": "https://goskive.com/course/fu-course-125",
      "slug": "fu-course-125",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 193,
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
      "updated_at": "2016-11-16T17:41:19.865Z",
      "shortname": "fu-course-125",
      "topic_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 125",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 596,
      "id": 181,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 194,
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
      "updated_at": "2016-11-16T17:41:19.904Z",
      "shortname": "fu-course-126",
      "topic_id": 193,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 597,
      "id": 182,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 195,
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
      "updated_at": "2016-11-16T17:41:19.953Z",
      "shortname": "fu-course-127",
      "topic_id": 194,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 597,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 196,
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
      "updated_at": "2016-11-16T17:41:19.996Z",
      "shortname": "fu-course-128",
      "topic_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41e2240243f5f474612d8000652c60a61f3430fe26f84958729243442e0c9ade"
```
