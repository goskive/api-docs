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
DELETE /v2/chapters/48
Content-Type: application/json
Authorization: Bearer 76d8b81284204ce9c471d0c94bdc436514f5ccfbadb38e28fee9e465f603f51b
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76d8b81284204ce9c471d0c94bdc436514f5ccfbadb38e28fee9e465f603f51b"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/44
Content-Type: application/json
Authorization: Bearer eba8a82e88261f7ede96df80a36bbe8e1c5b240f3336f5852cf0a12bf171b2a7
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
    "id": 44,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T09:19:06.212Z",
    "course_id": 56,
    "author_id": 199,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T09:19:05.711Z",
    "questions_updated_at": "2016-10-18T09:19:05.711Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 202,
        "chapter_id": 44,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:06.160Z",
        "created_at": "2016-10-18T09:19:06.160Z",
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
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 203,
        "chapter_id": 44,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:06.197Z",
        "created_at": "2016-10-18T09:19:06.197Z",
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
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 200,
        "chapter_id": 44,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:05.914Z",
        "created_at": "2016-10-18T09:19:05.812Z",
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
            "id": 111,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 112,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 201,
        "chapter_id": 44,
        "position": 57,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:06.095Z",
        "created_at": "2016-10-18T09:19:05.983Z",
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
            "id": 113,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 114,
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
curl "api.goskive.com/v2/chapters/44" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eba8a82e88261f7ede96df80a36bbe8e1c5b240f3336f5852cf0a12bf171b2a7"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/51
Content-Type: application/json
Authorization: Bearer c500d0edfab3d45c7e535147d46e62a03ed797146016743de325f81833758177
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
    "id": 51,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T09:19:08.016Z",
    "course_id": 63,
    "author_id": 227,
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
curl "api.goskive.com/v2/chapters/51" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c500d0edfab3d45c7e535147d46e62a03ed797146016743de325f81833758177"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/21
Content-Type: application/json
Authorization: Bearer a45639183d29b3a048590b4a1c52973c2e45926a5b92d88e3e829145bd0e6d17
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a45639183d29b3a048590b4a1c52973c2e45926a5b92d88e3e829145bd0e6d17"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 427a22ac49f4f40628c6a55bf96780d4cb3516f47a156d3ca485f360ec1045f2
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
      "id": 39,
      "author_id": 694,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:38.835Z",
      "status": "published",
      "subject_id": 227,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 696,
      "reply_to_id": 39,
      "created_at": "2016-10-18T09:19:38.914Z",
      "status": "published",
      "subject_id": 228,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 698,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:38.994Z",
      "status": "published",
      "subject_id": 229,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 700,
      "reply_to_id": 41,
      "created_at": "2016-10-18T09:19:39.073Z",
      "status": "published",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 702,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:39.152Z",
      "status": "reported",
      "subject_id": 231,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 704,
      "reply_to_id": 43,
      "created_at": "2016-10-18T09:19:39.232Z",
      "status": "published",
      "subject_id": 232,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 706,
      "reply_to_id": 43,
      "created_at": "2016-10-18T09:19:39.314Z",
      "status": "published",
      "subject_id": 233,
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
	-H "Authorization: Bearer 427a22ac49f4f40628c6a55bf96780d4cb3516f47a156d3ca485f360ec1045f2"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d2d2174f866c3c67a3238612906ca62c5d285a6f8e212e3768c66e0121529bb7
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
      "id": 46,
      "author_id": 709,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:39.449Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 711,
      "reply_to_id": 46,
      "created_at": "2016-10-18T09:19:39.528Z",
      "status": "published",
      "subject_id": 235,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 713,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:39.609Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 715,
      "reply_to_id": 48,
      "created_at": "2016-10-18T09:19:39.690Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 717,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:39.772Z",
      "status": "reported",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 719,
      "reply_to_id": 50,
      "created_at": "2016-10-18T09:19:39.853Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 721,
      "reply_to_id": 50,
      "created_at": "2016-10-18T09:19:39.943Z",
      "status": "published",
      "subject_id": 240,
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
	-H "Authorization: Bearer d2d2174f866c3c67a3238612906ca62c5d285a6f8e212e3768c66e0121529bb7"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer fd6aa5cf050b793477bec9e16a0a14e26a38d8a6e1b89a6e8bf8998534ceb910
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
      "id": 26,
      "author_id": 666,
      "reply_to_id": 25,
      "created_at": "2016-10-18T09:19:37.636Z",
      "status": "published",
      "subject_id": 214,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 670,
      "reply_to_id": 27,
      "created_at": "2016-10-18T09:19:37.800Z",
      "status": "published",
      "subject_id": 216,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 674,
      "reply_to_id": 29,
      "created_at": "2016-10-18T09:19:37.971Z",
      "status": "published",
      "subject_id": 218,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 676,
      "reply_to_id": 29,
      "created_at": "2016-10-18T09:19:38.051Z",
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
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd6aa5cf050b793477bec9e16a0a14e26a38d8a6e1b89a6e8bf8998534ceb910"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer fa5e6ae25d94f3cdd4ce49b1eda13ab8d40e7476c1131d22e08205d9981f6566
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
      "id": 57,
      "author_id": 732,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:40.421Z",
      "status": "reported",
      "subject_id": 245,
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
	-H "Authorization: Bearer fa5e6ae25d94f3cdd4ce49b1eda13ab8d40e7476c1131d22e08205d9981f6566"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/24/republish
Content-Type: application/json
Authorization: Bearer 75792717b0f1f85c185df37db990ebfbd94b3075e0451e8641839c5855855070
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/24/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75792717b0f1f85c185df37db990ebfbd94b3075e0451e8641839c5855855070"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/103/chapters
Content-Type: application/json
Authorization: Bearer 0f0de3b71d7e411edfc857d764944fab7829ae74c7809457345ea551221e2ac4
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
    "id": 74,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:19:18.517Z",
    "course_id": 103,
    "author_id": 372,
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
curl "api.goskive.com/v2/courses/103/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f0de3b71d7e411edfc857d764944fab7829ae74c7809457345ea551221e2ac4"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 79fc96be72248db3ce9ab5a7daad7d7ea5e094bc573cb10c46a71d0e5238630d
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
    "id": 76,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:19:18.885Z",
    "course_id": 106,
    "author_id": 378,
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
	-H "Authorization: Bearer 79fc96be72248db3ce9ab5a7daad7d7ea5e094bc573cb10c46a71d0e5238630d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 03382e5d795366cbcc5407e86da9cf7c69f59d86bf0962b2e99f27fbf70603e2
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
      "id": 86,
      "title": "Clever Chapter Title 65",
      "position": 1,
      "updated_at": "2016-10-18T09:19:20.003Z",
      "course_id": 112,
      "author_id": 401,
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
      "id": 87,
      "title": "Clever Chapter Title 66",
      "position": 2,
      "updated_at": "2016-10-18T09:19:20.028Z",
      "course_id": 112,
      "author_id": 402,
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
      "id": 88,
      "title": "Clever Chapter Title 67",
      "position": 3,
      "updated_at": "2016-10-18T09:19:20.274Z",
      "course_id": 112,
      "author_id": 403,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T09:19:19.921Z",
      "questions_updated_at": "2016-10-18T09:19:19.921Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03382e5d795366cbcc5407e86da9cf7c69f59d86bf0962b2e99f27fbf70603e2"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fe1e88f05eef7284f9a5cc120deaeab32e58b8eb1b588d5fb78cea6439fa177e
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
      "title": "Clever Chapter Title 68",
      "position": 1,
      "updated_at": "2016-10-18T09:19:20.412Z",
      "course_id": 113,
      "author_id": 408,
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
      "id": 90,
      "title": "Clever Chapter Title 69",
      "position": 2,
      "updated_at": "2016-10-18T09:19:20.438Z",
      "course_id": 113,
      "author_id": 409,
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
      "id": 91,
      "title": "Clever Chapter Title 70",
      "position": 3,
      "updated_at": "2016-10-18T09:19:20.463Z",
      "course_id": 113,
      "author_id": 410,
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
	-H "Authorization: Bearer fe1e88f05eef7284f9a5cc120deaeab32e58b8eb1b588d5fb78cea6439fa177e"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ff64b839a37979d6aa0efcb5ad0b36123556ff6f7d4669716f0d6425969ecdb6
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
	-H "Authorization: Bearer ff64b839a37979d6aa0efcb5ad0b36123556ff6f7d4669716f0d6425969ecdb6"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/10
Content-Type: application/json
Authorization: Bearer 2857bb98bd19b10a6e798cd7fdcf058937b3248a63966c38a47622204189b1e3
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2857bb98bd19b10a6e798cd7fdcf058937b3248a63966c38a47622204189b1e3"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 1c94f3934ad8d2b7667420e0c62381e41aefa48e8649d07498599806caf96aac
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
    "creator_id": 29,
    "id": 12,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 12,
    "additional_university_ids": [

    ],
    "topic_id": 12,
    "discipline_id": 12,
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
    "chapters_updated_at": "2016-10-18T09:18:46.191Z",
    "updated_at": "2016-10-18T09:18:47.590Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 7,
        "title": "Clever Chapter Title 7",
        "position": 1,
        "updated_at": "2016-10-18T09:18:47.546Z",
        "course_id": 12,
        "author_id": 29,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T09:18:46.191Z",
        "questions_updated_at": "2016-10-18T09:18:46.191Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 8,
        "title": "Clever Chapter Title 8",
        "position": 2,
        "updated_at": "2016-10-18T09:18:47.583Z",
        "course_id": 12,
        "author_id": 29,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T09:18:46.191Z",
        "questions_updated_at": "2016-10-18T09:18:46.191Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 29,
        "chapter_id": 7,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.387Z",
        "created_at": "2016-10-18T09:18:47.387Z",
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
        "author_id": 29,
        "chapter_id": 8,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.453Z",
        "created_at": "2016-10-18T09:18:47.453Z",
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
        "author_id": 29,
        "chapter_id": 7,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.424Z",
        "created_at": "2016-10-18T09:18:47.424Z",
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
        "author_id": 29,
        "chapter_id": 8,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.498Z",
        "created_at": "2016-10-18T09:18:47.498Z",
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
        "author_id": 32,
        "chapter_id": 7,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.536Z",
        "created_at": "2016-10-18T09:18:47.536Z",
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
        "author_id": 33,
        "chapter_id": 8,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.573Z",
        "created_at": "2016-10-18T09:18:47.573Z",
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
	-H "Authorization: Bearer 1c94f3934ad8d2b7667420e0c62381e41aefa48e8649d07498599806caf96aac"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/19
Content-Type: application/json
Authorization: Bearer d3dc1cfa04bcafbaf4a66fb9e797f5c73209fad6b58234262274dc11647908d9
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
    "creator_id": 53,
    "id": 19,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 19,
    "additional_university_ids": [

    ],
    "topic_id": 19,
    "discipline_id": 19,
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
    "updated_at": "2016-10-18T09:18:51.296Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/19" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3dc1cfa04bcafbaf4a66fb9e797f5c73209fad6b58234262274dc11647908d9"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 172675f6df8586867ac9fb55d7202f5fa5d26bb24e4418c00c6575c98cb648e6
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
    "creator_id": 48,
    "id": 16,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 16,
    "additional_university_ids": [

    ],
    "topic_id": 16,
    "discipline_id": 16,
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
    "updated_at": "2016-10-18T09:18:50.932Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 172675f6df8586867ac9fb55d7202f5fa5d26bb24e4418c00c6575c98cb648e6"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer acbde51aea4cc186cdcf7db846f0c96c1aa8eab2075bf11befe6f3f733c7f739
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
      "id": 19,
      "user_id": 742,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:40.977Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 20,
      "user_id": 746,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:41.290Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 750,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:41.567Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 754,
      "feedbackable_id": 94,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:41.850Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 758,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T09:19:42.131Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer acbde51aea4cc186cdcf7db846f0c96c1aa8eab2075bf11befe6f3f733c7f739"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 5929609f9fadd56726bba868cbbf74f2f2657de010f8a9d4566ace9703e9eff8
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
      "id": 37,
      "user_id": 816,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T09:19:46.245Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5929609f9fadd56726bba868cbbf74f2f2657de010f8a9d4566ace9703e9eff8"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Authorization: Bearer b0f821a15766f8860378401a36a51353317611d18d5c2a7e9c7db5a0199ac2fd
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
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Authorization: Bearer b0f821a15766f8860378401a36a51353317611d18d5c2a7e9c7db5a0199ac2fd" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/46/feedbacks
Content-Type: application/json
Authorization: Bearer 554d812c2ed8b21cd839b632a325803b725f8edd5307d13a4f9f5970cab82ea4
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
      "id": 7,
      "user_id": 303,
      "feedbackable_id": 46,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:13.408Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 302,
      "feedbackable_id": 46,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:13.397Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/46/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 554d812c2ed8b21cd839b632a325803b725f8edd5307d13a4f9f5970cab82ea4"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 57b332d8bf32966f07fa09b2c67697cb567a4f74f29c52e3e2dd7997a931feaf
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 465,
      "chapter_id": 109,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:23.569Z",
      "created_at": "2016-10-18T09:19:23.569Z",
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 468,
      "chapter_id": 110,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:23.700Z",
      "created_at": "2016-10-18T09:19:23.700Z",
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 471,
      "chapter_id": 111,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:23.831Z",
      "created_at": "2016-10-18T09:19:23.831Z",
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
      "author_id": 474,
      "chapter_id": 112,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:23.957Z",
      "created_at": "2016-10-18T09:19:23.957Z",
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
      "author_id": 477,
      "chapter_id": 113,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:24.088Z",
      "created_at": "2016-10-18T09:19:24.088Z",
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
	-H "Authorization: Bearer 57b332d8bf32966f07fa09b2c67697cb567a4f74f29c52e3e2dd7997a931feaf"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer d8f82936612ea694581919b9a87b4e15a4ec7e8dc022253e6a694176336ea12e
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 461,
      "chapter_id": 108,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:23.395Z",
      "created_at": "2016-10-18T09:19:23.395Z",
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
	-H "Authorization: Bearer d8f82936612ea694581919b9a87b4e15a4ec7e8dc022253e6a694176336ea12e"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/81/republish
Content-Type: application/json
Authorization: Bearer 0286019c5bfb45a525569b401cbc8271869a372e0508e6a9e59de48d6a88e13d
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/81/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0286019c5bfb45a525569b401cbc8271869a372e0508e6a9e59de48d6a88e13d"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/83/feedbacks
Content-Type: application/json
Authorization: Bearer 5b2ff2655cec1271fcc6d4037c1be33cfe51cc35952d7c82281b80acd5596dc2
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
      "id": 12,
      "user_id": 610,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:33.635Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 609,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:33.624Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b2ff2655cec1271fcc6d4037c1be33cfe51cc35952d7c82281b80acd5596dc2"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer fa33bec1e08c1618b33a6c233875bc9a397566b341fbaedda75ad37ed3623f82
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
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 889,
      "chapter_id": 178,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:51.387Z",
      "created_at": "2016-10-18T09:19:51.276Z",
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
          "id": 237,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 238,
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
      "author_id": 892,
      "chapter_id": 179,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:51.658Z",
      "created_at": "2016-10-18T09:19:51.546Z",
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
          "id": 239,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 240,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 116,
      "obfuscated_id": "PhHGVKqnHFA",
      "author_id": 886,
      "chapter_id": 177,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:51.117Z",
      "created_at": "2016-10-18T09:19:51.008Z",
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
          "id": 235,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 236,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 119,
      "obfuscated_id": "JRh8sWka24Y",
      "author_id": 895,
      "chapter_id": 180,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:51.956Z",
      "created_at": "2016-10-18T09:19:51.844Z",
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
          "id": 241,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 242,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 120,
      "obfuscated_id": "vEr9LtFjURM",
      "author_id": 898,
      "chapter_id": 181,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:52.216Z",
      "created_at": "2016-10-18T09:19:52.110Z",
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
          "id": 243,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 244,
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
	-H "Authorization: Bearer fa33bec1e08c1618b33a6c233875bc9a397566b341fbaedda75ad37ed3623f82"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c466ce036e4525bcd9ba51c8646606d46d22e4cdae16ec57d964909bb4e842b2
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
      "id": 130,
      "obfuscated_id": "N-qIf0IsvWM",
      "author_id": 930,
      "chapter_id": 191,
      "position": 121,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:55.011Z",
      "created_at": "2016-10-18T09:19:54.902Z",
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
          "id": 263,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 264,
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
	-H "Authorization: Bearer c466ce036e4525bcd9ba51c8646606d46d22e4cdae16ec57d964909bb4e842b2"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/114/republish
Content-Type: application/json
Authorization: Bearer aab725a557e4716995e2625f7c8999da285ed22384a8707efb1c042ab6daa9dd
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aab725a557e4716995e2625f7c8999da285ed22384a8707efb1c042ab6daa9dd"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b3f7938ce06fc2f48029ea7f1d0ac9251c462fe877bf20adb23fb5ee4bc85fc6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":200,"published":false}}
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
    "creator_id": 591,
    "id": 191,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "topic_id": 200,
    "discipline_id": 201,
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
    "updated_at": "2016-10-18T09:19:31.961Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":200,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3f7938ce06fc2f48029ea7f1d0ac9251c462fe877bf20adb23fb5ee4bc85fc6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f1475b4c8c68f6773bc73878aa63bd084aa8e8e88e40f44eafa14d9bdb0ea9bb
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
      "creator_id": 549,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-96",
      "html_url": "https://goskive.com/course/fu-course-96",
      "slug": "fu-course-96",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 163,
      "discipline_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 96",
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
      "updated_at": "2016-10-18T09:19:28.066Z",
      "shortname": "fu-course-96"
    },
    {
      "creator_id": 549,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-97",
      "html_url": "https://goskive.com/course/fu-course-97",
      "slug": "fu-course-97",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 164,
      "discipline_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 97",
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
      "updated_at": "2016-10-18T09:19:28.107Z",
      "shortname": "fu-course-97"
    },
    {
      "creator_id": 550,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "discipline_id": 166,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
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
      "updated_at": "2016-10-18T09:19:28.154Z",
      "shortname": "fu-course-98"
    },
    {
      "creator_id": 550,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-99",
      "html_url": "https://goskive.com/course/fu-course-99",
      "slug": "fu-course-99",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 167,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 99",
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
      "chapters_updated_at": "2016-10-18T09:19:28.434Z",
      "updated_at": "2016-10-18T09:19:28.441Z",
      "shortname": "fu-course-99"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1475b4c8c68f6773bc73878aa63bd084aa8e8e88e40f44eafa14d9bdb0ea9bb"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4e1ad133a7b3bd3e8af1a11a75862fe159da68766f71e1e1a5e950f8dd8f8bc0
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
      "creator_id": 555,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-100",
      "html_url": "https://goskive.com/course/fu-course-100",
      "slug": "fu-course-100",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 167,
      "discipline_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 100",
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
      "updated_at": "2016-10-18T09:19:28.596Z",
      "shortname": "fu-course-100"
    },
    {
      "creator_id": 555,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-101",
      "html_url": "https://goskive.com/course/fu-course-101",
      "slug": "fu-course-101",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 168,
      "discipline_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 101",
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
      "updated_at": "2016-10-18T09:19:28.635Z",
      "shortname": "fu-course-101"
    },
    {
      "creator_id": 556,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 169,
      "discipline_id": 170,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
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
      "updated_at": "2016-10-18T09:19:28.687Z",
      "shortname": "fu-course-102"
    },
    {
      "creator_id": 556,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 170,
      "discipline_id": 171,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
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
      "updated_at": "2016-10-18T09:19:28.729Z",
      "shortname": "fu-course-103"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e1ad133a7b3bd3e8af1a11a75862fe159da68766f71e1e1a5e950f8dd8f8bc0"
```
