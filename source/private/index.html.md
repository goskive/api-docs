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
DELETE /v2/chapters/135
Content-Type: application/json
Authorization: Bearer 90982668137ce5bfad166fc161e6115fb23f7ef50ad5acad477b06fecea1f650
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/135" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90982668137ce5bfad166fc161e6115fb23f7ef50ad5acad477b06fecea1f650"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/134
Content-Type: application/json
Authorization: Bearer b936a3cbc146f19c497e890f8e0adb5a6497c236d4abe40800554b704ae9b602
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
    "id": 134,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T12:25:46.267Z",
    "course_id": 234,
    "author_id": 661,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T12:25:45.679Z",
    "questions_updated_at": "2016-10-18T12:25:45.679Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 664,
        "chapter_id": 134,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:46.207Z",
        "created_at": "2016-10-18T12:25:46.207Z",
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
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 665,
        "chapter_id": 134,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:46.249Z",
        "created_at": "2016-10-18T12:25:46.249Z",
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
        "id": 98,
        "obfuscated_id": "icApzX10lRE",
        "author_id": 662,
        "chapter_id": 134,
        "position": 85,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:45.919Z",
        "created_at": "2016-10-18T12:25:45.799Z",
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
            "id": 199,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 200,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 663,
        "chapter_id": 134,
        "position": 86,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:46.129Z",
        "created_at": "2016-10-18T12:25:45.999Z",
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
            "id": 201,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 202,
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
curl "api.goskive.com/v2/chapters/134" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b936a3cbc146f19c497e890f8e0adb5a6497c236d4abe40800554b704ae9b602"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/139
Content-Type: application/json
Authorization: Bearer 6ed2e229aa8874b26fc112c4fcd4bdb57b3499f9da61524d10f9aa546cf5322b
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
    "id": 139,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T12:25:47.535Z",
    "course_id": 239,
    "author_id": 680,
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
curl "api.goskive.com/v2/chapters/139" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ed2e229aa8874b26fc112c4fcd4bdb57b3499f9da61524d10f9aa546cf5322b"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/44
Content-Type: application/json
Authorization: Bearer f2d41772c0733610d4dc18de5e5428d47dad33074fdc7ed27e61c69bed9c1c75
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2d41772c0733610d4dc18de5e5428d47dad33074fdc7ed27e61c69bed9c1c75"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d7f3a454bee3b0b6feae7a3d7ddaf2e3f11461ef89195efc176b951a4314e371
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
      "id": 20,
      "author_id": 171,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:58.123Z",
      "status": "published",
      "subject_id": 52,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 173,
      "reply_to_id": 20,
      "created_at": "2016-10-18T12:24:58.216Z",
      "status": "published",
      "subject_id": 53,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 175,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:58.308Z",
      "status": "published",
      "subject_id": 54,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 177,
      "reply_to_id": 22,
      "created_at": "2016-10-18T12:24:58.399Z",
      "status": "published",
      "subject_id": 55,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 179,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:58.493Z",
      "status": "reported",
      "subject_id": 56,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 181,
      "reply_to_id": 24,
      "created_at": "2016-10-18T12:24:58.591Z",
      "status": "published",
      "subject_id": 57,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 183,
      "reply_to_id": 24,
      "created_at": "2016-10-18T12:24:58.697Z",
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
	-H "Authorization: Bearer d7f3a454bee3b0b6feae7a3d7ddaf2e3f11461ef89195efc176b951a4314e371"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 51b6c0c4d8cd5dad9edcde5d72dda0e19e684effac390cf9729f350b6c195d65
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
      "author_id": 201,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:59.566Z",
      "status": "published",
      "subject_id": 66,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 203,
      "reply_to_id": 34,
      "created_at": "2016-10-18T12:24:59.658Z",
      "status": "published",
      "subject_id": 67,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 205,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:59.748Z",
      "status": "published",
      "subject_id": 68,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 207,
      "reply_to_id": 36,
      "created_at": "2016-10-18T12:24:59.841Z",
      "status": "published",
      "subject_id": 69,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 209,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:59.941Z",
      "status": "reported",
      "subject_id": 70,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 211,
      "reply_to_id": 38,
      "created_at": "2016-10-18T12:25:00.035Z",
      "status": "published",
      "subject_id": 71,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 213,
      "reply_to_id": 38,
      "created_at": "2016-10-18T12:25:00.154Z",
      "status": "published",
      "subject_id": 72,
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
	-H "Authorization: Bearer 51b6c0c4d8cd5dad9edcde5d72dda0e19e684effac390cf9729f350b6c195d65"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer cb1dd4de42916bb74a8a0491f594651f46fdb13433c285ed9be57728a1bf8597
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
      "id": 28,
      "author_id": 188,
      "reply_to_id": 27,
      "created_at": "2016-10-18T12:24:58.953Z",
      "status": "published",
      "subject_id": 60,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 192,
      "reply_to_id": 29,
      "created_at": "2016-10-18T12:24:59.137Z",
      "status": "published",
      "subject_id": 62,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 196,
      "reply_to_id": 31,
      "created_at": "2016-10-18T12:24:59.321Z",
      "status": "published",
      "subject_id": 64,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 198,
      "reply_to_id": 31,
      "created_at": "2016-10-18T12:24:59.416Z",
      "status": "published",
      "subject_id": 65,
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
	-H "Authorization: Bearer cb1dd4de42916bb74a8a0491f594651f46fdb13433c285ed9be57728a1bf8597"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 496e4adf922ef981a4529ac791c000084b6ca1baf05606aa516e1e4d9ed1525f
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
      "id": 10,
      "author_id": 149,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:24:57.103Z",
      "status": "reported",
      "subject_id": 42,
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
	-H "Authorization: Bearer 496e4adf922ef981a4529ac791c000084b6ca1baf05606aa516e1e4d9ed1525f"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer e44501b2c74d3cf57274d39bbc39ddff96e491019a198766163ef69928e83c40
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e44501b2c74d3cf57274d39bbc39ddff96e491019a198766163ef69928e83c40"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 08b16503f8fe230bb54a41cfd29bbedd77680fb6cc380f4188e0e619de5765c7
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
    "id": 9,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:24:48.580Z",
    "course_id": 12,
    "author_id": 36,
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
	-H "Authorization: Bearer 08b16503f8fe230bb54a41cfd29bbedd77680fb6cc380f4188e0e619de5765c7"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/13/chapters
Content-Type: application/json
Authorization: Bearer 253373a7579a84a2b79f6630e2320af808605918dbd5fa6d39f262e721711788
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
    "id": 10,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:24:48.749Z",
    "course_id": 13,
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
curl "api.goskive.com/v2/courses/13/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 253373a7579a84a2b79f6630e2320af808605918dbd5fa6d39f262e721711788"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7a7d1c75fddbb9fb8842b392ea4182df4edf7fe00961e8e648da65eeb6dbc64a
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
      "id": 14,
      "title": "Clever Chapter Title 11",
      "position": 1,
      "updated_at": "2016-10-18T12:24:49.169Z",
      "course_id": 16,
      "author_id": 47,
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
      "id": 15,
      "title": "Clever Chapter Title 12",
      "position": 2,
      "updated_at": "2016-10-18T12:24:49.193Z",
      "course_id": 16,
      "author_id": 48,
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
      "id": 16,
      "title": "Clever Chapter Title 13",
      "position": 3,
      "updated_at": "2016-10-18T12:24:49.466Z",
      "course_id": 16,
      "author_id": 49,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T12:24:49.093Z",
      "questions_updated_at": "2016-10-18T12:24:49.093Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a7d1c75fddbb9fb8842b392ea4182df4edf7fe00961e8e648da65eeb6dbc64a"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f71d6899a71f92aa8991128a388959c60079e303d24c485f1bd720179de1ed50
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
      "id": 17,
      "title": "Clever Chapter Title 14",
      "position": 1,
      "updated_at": "2016-10-18T12:24:49.617Z",
      "course_id": 17,
      "author_id": 54,
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
      "id": 18,
      "title": "Clever Chapter Title 15",
      "position": 2,
      "updated_at": "2016-10-18T12:24:49.642Z",
      "course_id": 17,
      "author_id": 55,
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
      "id": 19,
      "title": "Clever Chapter Title 16",
      "position": 3,
      "updated_at": "2016-10-18T12:24:49.668Z",
      "course_id": 17,
      "author_id": 56,
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
	-H "Authorization: Bearer f71d6899a71f92aa8991128a388959c60079e303d24c485f1bd720179de1ed50"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6e8fea1598ef69df466c78129f5428a322e888e4f550581853fdd201d339d996
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
	-H "Authorization: Bearer 6e8fea1598ef69df466c78129f5428a322e888e4f550581853fdd201d339d996"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/202
Content-Type: application/json
Authorization: Bearer 76778448c77ec883a231034146befff0d5524f8b40ff52346a88b39d3f44787c
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/202" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76778448c77ec883a231034146befff0d5524f8b40ff52346a88b39d3f44787c"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 0c984d186ca871122e772fc90cb2b4dc7ab8b07e3b1c65fb32f7989d04f2872a
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
    "creator_id": 564,
    "id": 206,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 190,
    "additional_university_ids": [

    ],
    "topic_id": 213,
    "discipline_id": 214,
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
    "chapters_updated_at": "2016-10-18T12:25:33.637Z",
    "updated_at": "2016-10-18T12:25:35.416Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 119,
        "title": "Clever Chapter Title 110",
        "position": 1,
        "updated_at": "2016-10-18T12:25:35.361Z",
        "course_id": 206,
        "author_id": 564,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T12:25:33.637Z",
        "questions_updated_at": "2016-10-18T12:25:33.637Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 120,
        "title": "Clever Chapter Title 111",
        "position": 2,
        "updated_at": "2016-10-18T12:25:35.407Z",
        "course_id": 206,
        "author_id": 564,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T12:25:33.637Z",
        "questions_updated_at": "2016-10-18T12:25:33.637Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 564,
        "chapter_id": 119,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.168Z",
        "created_at": "2016-10-18T12:25:35.168Z",
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
        "author_id": 564,
        "chapter_id": 120,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.253Z",
        "created_at": "2016-10-18T12:25:35.253Z",
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
        "author_id": 564,
        "chapter_id": 119,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.216Z",
        "created_at": "2016-10-18T12:25:35.216Z",
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
        "author_id": 564,
        "chapter_id": 120,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.302Z",
        "created_at": "2016-10-18T12:25:35.302Z",
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
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 567,
        "chapter_id": 119,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.348Z",
        "created_at": "2016-10-18T12:25:35.348Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 568,
        "chapter_id": 120,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.394Z",
        "created_at": "2016-10-18T12:25:35.394Z",
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
	-H "Authorization: Bearer 0c984d186ca871122e772fc90cb2b4dc7ab8b07e3b1c65fb32f7989d04f2872a"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/209
Content-Type: application/json
Authorization: Bearer c5728a12f8890a2ec6badd068412d3dc1c486c9570b773bd3daaa9e2b51b3dab
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
    "creator_id": 577,
    "id": 209,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 193,
    "additional_university_ids": [

    ],
    "topic_id": 216,
    "discipline_id": 217,
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
    "updated_at": "2016-10-18T12:25:37.558Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/209" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5728a12f8890a2ec6badd068412d3dc1c486c9570b773bd3daaa9e2b51b3dab"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ce191014356aee6b9b5115c7bc660af76b8abd67c45af8aba5c13465a2018288
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
    "creator_id": 580,
    "id": 211,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 195,
    "additional_university_ids": [

    ],
    "topic_id": 218,
    "discipline_id": 219,
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
    "updated_at": "2016-10-18T12:25:37.849Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce191014356aee6b9b5115c7bc660af76b8abd67c45af8aba5c13465a2018288"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 1fea4131944fdd1509d04af0b24ba7ee73cc70f1b835a81aa0091566541f1cc8
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
      "id": 20,
      "user_id": 767,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:54.343Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 771,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:54.671Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 775,
      "feedbackable_id": 118,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:55.007Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 779,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:55.351Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 783,
      "feedbackable_id": 120,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T12:25:55.689Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fea4131944fdd1509d04af0b24ba7ee73cc70f1b835a81aa0091566541f1cc8"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer adb52c7d833ca8eaf019ed96c0a0dc8be78f8c714200dfe807339aee41b82014
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
      "id": 10,
      "user_id": 725,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T12:25:50.915Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adb52c7d833ca8eaf019ed96c0a0dc8be78f8c714200dfe807339aee41b82014"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Authorization: Bearer 7199ed8848838b913c81206c2dadc69a4c4ef0e9edaf043a6159fc6ac89dbc52
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
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Authorization: Bearer 7199ed8848838b913c81206c2dadc69a4c4ef0e9edaf043a6159fc6ac89dbc52" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/92/feedbacks
Content-Type: application/json
Authorization: Bearer a83bb25b683c86bb6553d157bdb91012d691c4c1a54b5f46456d456b772cc9c0
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
      "user_id": 942,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:26:08.362Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 941,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:26:08.351Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/92/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a83bb25b683c86bb6553d157bdb91012d691c4c1a54b5f46456d456b772cc9c0"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 90fa003377799031302805c1f71aadfd73d26611c6be11fb3a3e0435094ff538
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 482,
      "chapter_id": 96,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:24.843Z",
      "created_at": "2016-10-18T12:25:24.843Z",
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
      "author_id": 485,
      "chapter_id": 97,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:24.990Z",
      "created_at": "2016-10-18T12:25:24.990Z",
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 488,
      "chapter_id": 98,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:25.136Z",
      "created_at": "2016-10-18T12:25:25.136Z",
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 491,
      "chapter_id": 99,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:25.284Z",
      "created_at": "2016-10-18T12:25:25.284Z",
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 494,
      "chapter_id": 100,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:25.433Z",
      "created_at": "2016-10-18T12:25:25.433Z",
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
	-H "Authorization: Bearer 90fa003377799031302805c1f71aadfd73d26611c6be11fb3a3e0435094ff538"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer ddaf22e6824bdc00219c6c9385b41c572729715c7846c5c0508834746493b74e
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 510,
      "chapter_id": 105,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:26.239Z",
      "created_at": "2016-10-18T12:25:26.239Z",
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
	-H "Authorization: Bearer ddaf22e6824bdc00219c6c9385b41c572729715c7846c5c0508834746493b74e"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/43/republish
Content-Type: application/json
Authorization: Bearer 13f418723ea77cc06d08f97baf2809ccda77511441bf9c123a01d9f1ba0206d9
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13f418723ea77cc06d08f97baf2809ccda77511441bf9c123a01d9f1ba0206d9"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/121/feedbacks
Content-Type: application/json
Authorization: Bearer a04f002e1f66b003730fcfc9af5799d513680b35554d51a12b2f4662b66ee4a9
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
      "id": 32,
      "user_id": 822,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:57.860Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 821,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:57.848Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/121/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a04f002e1f66b003730fcfc9af5799d513680b35554d51a12b2f4662b66ee4a9"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer afdb5e617265d536b64472951a6edbee89e813b1a7c3c9385c5db549c34ef660
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
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 393,
      "chapter_id": 71,
      "position": 38,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:16.598Z",
      "created_at": "2016-10-18T12:25:16.456Z",
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
          "id": 86,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 87,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 384,
      "chapter_id": 68,
      "position": 35,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:15.662Z",
      "created_at": "2016-10-18T12:25:15.529Z",
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
          "id": 80,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 81,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 387,
      "chapter_id": 69,
      "position": 36,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:15.970Z",
      "created_at": "2016-10-18T12:25:15.836Z",
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
          "id": 82,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 83,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 390,
      "chapter_id": 70,
      "position": 37,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:16.282Z",
      "created_at": "2016-10-18T12:25:16.147Z",
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
          "id": 84,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 85,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 396,
      "chapter_id": 72,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:16.904Z",
      "created_at": "2016-10-18T12:25:16.774Z",
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
          "id": 88,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 89,
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
	-H "Authorization: Bearer afdb5e617265d536b64472951a6edbee89e813b1a7c3c9385c5db549c34ef660"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer cdd7ee074b3827ec88fec51160b0691452d78eb74090963c65ef240d24d49a3a
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 412,
      "chapter_id": 77,
      "position": 44,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:18.580Z",
      "created_at": "2016-10-18T12:25:18.448Z",
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
          "id": 98,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 99,
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
	-H "Authorization: Bearer cdd7ee074b3827ec88fec51160b0691452d78eb74090963c65ef240d24d49a3a"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/36/republish
Content-Type: application/json
Authorization: Bearer 2c6ec1a58d04e256751a27d7f26516adcba5478f2352867606fc1ff15965eeb5
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/36/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c6ec1a58d04e256751a27d7f26516adcba5478f2352867606fc1ff15965eeb5"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5adb93929e0477578c600c65821913cda7351e454f70828e271cb4388d93c2a6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":131,"published":false}}
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
    "creator_id": 323,
    "id": 129,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 108,
    "additional_university_ids": [

    ],
    "topic_id": 131,
    "discipline_id": 131,
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
    "updated_at": "2016-10-18T12:25:09.604Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":131,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5adb93929e0477578c600c65821913cda7351e454f70828e271cb4388d93c2a6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1e474985e50abf91b0b9503efa044e67e9f6424618fcca605a82e41cddd93f29
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
      "creator_id": 309,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-93",
      "html_url": "https://goskive.com/course/fu-course-93",
      "slug": "fu-course-93",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 119,
      "discipline_id": 119,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 93",
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
      "updated_at": "2016-10-18T12:25:08.256Z",
      "shortname": "fu-course-93"
    },
    {
      "creator_id": 309,
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-94",
      "html_url": "https://goskive.com/course/fu-course-94",
      "slug": "fu-course-94",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 120,
      "discipline_id": 120,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 94",
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
      "updated_at": "2016-10-18T12:25:08.298Z",
      "shortname": "fu-course-94"
    },
    {
      "creator_id": 310,
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-95",
      "html_url": "https://goskive.com/course/fu-course-95",
      "slug": "fu-course-95",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 121,
      "discipline_id": 121,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 95",
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
      "updated_at": "2016-10-18T12:25:08.349Z",
      "shortname": "fu-course-95"
    },
    {
      "creator_id": 310,
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-96",
      "html_url": "https://goskive.com/course/fu-course-96",
      "slug": "fu-course-96",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 122,
      "discipline_id": 122,
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
      "chapters_updated_at": "2016-10-18T12:25:08.679Z",
      "updated_at": "2016-10-18T12:25:08.686Z",
      "shortname": "fu-course-96"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e474985e50abf91b0b9503efa044e67e9f6424618fcca605a82e41cddd93f29"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8f8368a46cb966e5b2c53c26ccda8c67113ae152424004ae4340c213f82fb1a4
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
      "creator_id": 316,
      "id": 121,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-97",
      "html_url": "https://goskive.com/course/fu-course-97",
      "slug": "fu-course-97",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 123,
      "discipline_id": 123,
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
      "updated_at": "2016-10-18T12:25:08.910Z",
      "shortname": "fu-course-97"
    },
    {
      "creator_id": 316,
      "id": 122,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 124,
      "discipline_id": 124,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-18T12:25:08.953Z",
      "shortname": "fu-course-98"
    },
    {
      "creator_id": 317,
      "id": 123,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-99",
      "html_url": "https://goskive.com/course/fu-course-99",
      "slug": "fu-course-99",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 125,
      "discipline_id": 125,
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
      "updated_at": "2016-10-18T12:25:09.005Z",
      "shortname": "fu-course-99"
    },
    {
      "creator_id": 317,
      "id": 124,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-100",
      "html_url": "https://goskive.com/course/fu-course-100",
      "slug": "fu-course-100",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 126,
      "discipline_id": 126,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-18T12:25:09.049Z",
      "shortname": "fu-course-100"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f8368a46cb966e5b2c53c26ccda8c67113ae152424004ae4340c213f82fb1a4"
```
