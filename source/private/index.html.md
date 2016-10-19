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
DELETE /v2/chapters/6
Content-Type: application/json
Authorization: Bearer 5e06458d9fac8af2634bbdc577cddd8211c8ce07e706449b5163ae5fa5ca8b33
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e06458d9fac8af2634bbdc577cddd8211c8ce07e706449b5163ae5fa5ca8b33"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 40517dac2f49faa49afed5cdfe1e84383414e760b7528c16dfd0ec1e46895f86
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
    "id": 9,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T11:44:44.093Z",
    "course_id": 9,
    "author_id": 29,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-19T11:44:43.541Z",
    "questions_updated_at": "2016-10-19T11:44:43.541Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 32,
        "chapter_id": 9,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:44.037Z",
        "created_at": "2016-10-19T11:44:44.037Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 33,
        "chapter_id": 9,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:44.075Z",
        "created_at": "2016-10-19T11:44:44.075Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 30,
        "chapter_id": 9,
        "position": 5,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:43.771Z",
        "created_at": "2016-10-19T11:44:43.658Z",
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
            "id": 9,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 10,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 31,
        "chapter_id": 9,
        "position": 6,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:43.966Z",
        "created_at": "2016-10-19T11:44:43.847Z",
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
            "id": 11,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 12,
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
curl "api.goskive.com/v2/chapters/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40517dac2f49faa49afed5cdfe1e84383414e760b7528c16dfd0ec1e46895f86"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/2
Content-Type: application/json
Authorization: Bearer f13b843b8a438e515f1a7b950cd33417aca396a2ca6b072b9512d44b7894293f
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
    "id": 2,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T11:44:41.635Z",
    "course_id": 2,
    "author_id": 4,
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
curl "api.goskive.com/v2/chapters/2" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f13b843b8a438e515f1a7b950cd33417aca396a2ca6b072b9512d44b7894293f"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/17
Content-Type: application/json
Authorization: Bearer 3ccd07cc3a0f9a8a98ba5cdaf85d1a20ca3736c0f0d340257adab24b9f04904f
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
	-H "Authorization: Bearer 3ccd07cc3a0f9a8a98ba5cdaf85d1a20ca3736c0f0d340257adab24b9f04904f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer fda8d61ba4fa1fa613dd6c8f7bf595c6a287b4854ff4954c1f265518d2cfb284
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
      "author_id": 748,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:41.281Z",
      "status": "published",
      "subject_id": 244,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 750,
      "reply_to_id": 32,
      "created_at": "2016-10-19T11:45:41.370Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 752,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:41.459Z",
      "status": "published",
      "subject_id": 246,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 754,
      "reply_to_id": 34,
      "created_at": "2016-10-19T11:45:41.548Z",
      "status": "published",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 756,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:41.638Z",
      "status": "reported",
      "subject_id": 248,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 758,
      "reply_to_id": 36,
      "created_at": "2016-10-19T11:45:41.730Z",
      "status": "published",
      "subject_id": 249,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 760,
      "reply_to_id": 36,
      "created_at": "2016-10-19T11:45:41.822Z",
      "status": "published",
      "subject_id": 250,
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
	-H "Authorization: Bearer fda8d61ba4fa1fa613dd6c8f7bf595c6a287b4854ff4954c1f265518d2cfb284"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 930963929904fc3cbddc87624ebad6bd2fae85c5ac2d5cc9c0b9d304e514ad84
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
      "author_id": 763,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:41.975Z",
      "status": "published",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 765,
      "reply_to_id": 39,
      "created_at": "2016-10-19T11:45:42.064Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 767,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:42.154Z",
      "status": "published",
      "subject_id": 253,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 769,
      "reply_to_id": 41,
      "created_at": "2016-10-19T11:45:42.252Z",
      "status": "published",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 771,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:42.341Z",
      "status": "reported",
      "subject_id": 255,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 773,
      "reply_to_id": 43,
      "created_at": "2016-10-19T11:45:42.439Z",
      "status": "published",
      "subject_id": 256,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 775,
      "reply_to_id": 43,
      "created_at": "2016-10-19T11:45:42.535Z",
      "status": "published",
      "subject_id": 257,
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
	-H "Authorization: Bearer 930963929904fc3cbddc87624ebad6bd2fae85c5ac2d5cc9c0b9d304e514ad84"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer c9ba235637ba9d62f44628e40d74f12298f4bb5a3a8635f48c120aa71057226f
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
      "id": 19,
      "author_id": 720,
      "reply_to_id": 18,
      "created_at": "2016-10-19T11:45:39.964Z",
      "status": "published",
      "subject_id": 231,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 724,
      "reply_to_id": 20,
      "created_at": "2016-10-19T11:45:40.155Z",
      "status": "published",
      "subject_id": 233,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 728,
      "reply_to_id": 22,
      "created_at": "2016-10-19T11:45:40.335Z",
      "status": "published",
      "subject_id": 235,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 730,
      "reply_to_id": 22,
      "created_at": "2016-10-19T11:45:40.453Z",
      "status": "published",
      "subject_id": 236,
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
	-H "Authorization: Bearer c9ba235637ba9d62f44628e40d74f12298f4bb5a3a8635f48c120aa71057226f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer fd198355dd2c382aca459e8ab1bc4f858359d4ac595ceb8b7f1c2b2d73e209a9
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
      "author_id": 741,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:40.974Z",
      "status": "reported",
      "subject_id": 241,
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
	-H "Authorization: Bearer fd198355dd2c382aca459e8ab1bc4f858359d4ac595ceb8b7f1c2b2d73e209a9"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/53/republish
Content-Type: application/json
Authorization: Bearer 76088d344bfaeb6de42d276a442d9368975b0b6ca3b3c006694134771f934bdc
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76088d344bfaeb6de42d276a442d9368975b0b6ca3b3c006694134771f934bdc"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2cbc0028380eb6a82d02d5cabd351b49390665c983cfcb98f51ac8ba71eab081
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
    "id": 42,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T11:44:59.518Z",
    "course_id": 80,
    "author_id": 172,
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
	-H "Authorization: Bearer 2cbc0028380eb6a82d02d5cabd351b49390665c983cfcb98f51ac8ba71eab081"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/82/chapters
Content-Type: application/json
Authorization: Bearer 3ca4631bce9a7c8966d883d728ff18e1beecb2b1ba075120e2f306fa9408125d
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
    "id": 44,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T11:44:59.783Z",
    "course_id": 82,
    "author_id": 176,
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
curl "api.goskive.com/v2/courses/82/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ca4631bce9a7c8966d883d728ff18e1beecb2b1ba075120e2f306fa9408125d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0abe3a726d2b090e8cf6cd2b01fbafa0cd395f822fa73e7c28fa1d2048119030
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
      "id": 45,
      "title": "Clever Chapter Title 30",
      "position": 1,
      "updated_at": "2016-10-19T11:44:59.889Z",
      "course_id": 83,
      "author_id": 178,
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
      "id": 46,
      "title": "Clever Chapter Title 31",
      "position": 2,
      "updated_at": "2016-10-19T11:44:59.913Z",
      "course_id": 83,
      "author_id": 179,
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
      "id": 47,
      "title": "Clever Chapter Title 32",
      "position": 3,
      "updated_at": "2016-10-19T11:45:00.164Z",
      "course_id": 83,
      "author_id": 180,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-19T11:44:59.814Z",
      "questions_updated_at": "2016-10-19T11:44:59.814Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0abe3a726d2b090e8cf6cd2b01fbafa0cd395f822fa73e7c28fa1d2048119030"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f701df4fbf7f9d020bfa2e97bd4b7d394407e98d0f19e1100fef2347705babee
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
      "id": 48,
      "title": "Clever Chapter Title 33",
      "position": 1,
      "updated_at": "2016-10-19T11:45:00.437Z",
      "course_id": 85,
      "author_id": 187,
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
      "id": 49,
      "title": "Clever Chapter Title 34",
      "position": 2,
      "updated_at": "2016-10-19T11:45:00.463Z",
      "course_id": 85,
      "author_id": 188,
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
      "id": 50,
      "title": "Clever Chapter Title 35",
      "position": 3,
      "updated_at": "2016-10-19T11:45:00.489Z",
      "course_id": 85,
      "author_id": 189,
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
	-H "Authorization: Bearer f701df4fbf7f9d020bfa2e97bd4b7d394407e98d0f19e1100fef2347705babee"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 878bc731be571f5f6eef3358b248654e806a177d6721b9a5c3dc520d2c13d584
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
	-H "Authorization: Bearer 878bc731be571f5f6eef3358b248654e806a177d6721b9a5c3dc520d2c13d584"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/290
Content-Type: application/json
Authorization: Bearer d67444d9085e3006187775f1ad3ff36da364890f929e4c8c8fb7f113b953e668
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/290" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d67444d9085e3006187775f1ad3ff36da364890f929e4c8c8fb7f113b953e668"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 76ef0b71d5bf0aec3ca9b6a505c7dc3f26c47b7781304036017a99c1f926409b
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
    "creator_id": 907,
    "id": 294,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 279,
    "additional_university_ids": [

    ],
    "topic_id": 301,
    "discipline_id": 302,
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
    "chapters_updated_at": "2016-10-19T11:45:54.322Z",
    "updated_at": "2016-10-19T11:45:55.947Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 183,
        "title": "Clever Chapter Title 159",
        "position": 1,
        "updated_at": "2016-10-19T11:45:55.899Z",
        "course_id": 294,
        "author_id": 907,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T11:45:54.322Z",
        "questions_updated_at": "2016-10-19T11:45:54.322Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 184,
        "title": "Clever Chapter Title 160",
        "position": 2,
        "updated_at": "2016-10-19T11:45:55.939Z",
        "course_id": 294,
        "author_id": 907,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T11:45:54.322Z",
        "questions_updated_at": "2016-10-19T11:45:54.322Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 907,
        "chapter_id": 183,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.724Z",
        "created_at": "2016-10-19T11:45:55.724Z",
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
        "author_id": 907,
        "chapter_id": 184,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.803Z",
        "created_at": "2016-10-19T11:45:55.803Z",
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
        "author_id": 907,
        "chapter_id": 183,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.768Z",
        "created_at": "2016-10-19T11:45:55.768Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 907,
        "chapter_id": 184,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.848Z",
        "created_at": "2016-10-19T11:45:55.848Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 910,
        "chapter_id": 183,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.889Z",
        "created_at": "2016-10-19T11:45:55.889Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 911,
        "chapter_id": 184,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:55.929Z",
        "created_at": "2016-10-19T11:45:55.929Z",
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
	-H "Authorization: Bearer 76ef0b71d5bf0aec3ca9b6a505c7dc3f26c47b7781304036017a99c1f926409b"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/281
Content-Type: application/json
Authorization: Bearer f08439a8b44b9c04abc0132055a9a07d68c508593bf33ccd0953c3a4926c5fdf
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
    "creator_id": 872,
    "id": 281,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 266,
    "additional_university_ids": [

    ],
    "topic_id": 288,
    "discipline_id": 289,
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
    "updated_at": "2016-10-19T11:45:49.291Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/281" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f08439a8b44b9c04abc0132055a9a07d68c508593bf33ccd0953c3a4926c5fdf"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 439c766f9040cc57609d7f1135c1ede9fa947aa7f63cdd888b5c3e188b3ac773
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
    "creator_id": 870,
    "id": 280,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 265,
    "additional_university_ids": [

    ],
    "topic_id": 287,
    "discipline_id": 288,
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
    "updated_at": "2016-10-19T11:45:49.146Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 439c766f9040cc57609d7f1135c1ede9fa947aa7f63cdd888b5c3e188b3ac773"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 2854f4c986b7c24fafba3d8d1e235d723c7023e9d14031cdb53472286c4017cc
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
      "id": 6,
      "user_id": 273,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:05.336Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 277,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:05.647Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 281,
      "feedbackable_id": 41,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:05.974Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 285,
      "feedbackable_id": 42,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:06.285Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 289,
      "feedbackable_id": 43,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T11:45:06.597Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2854f4c986b7c24fafba3d8d1e235d723c7023e9d14031cdb53472286c4017cc"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 189aec63fde9a9a35cb125e375ac9a7bd60b3d0ddf765a7467f41f8658e0c085
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
      "id": 24,
      "user_id": 347,
      "feedbackable_id": 57,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T11:45:10.927Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 189aec63fde9a9a35cb125e375ac9a7bd60b3d0ddf765a7467f41f8658e0c085"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/3
Content-Type: application/json
Authorization: Bearer 6440e7eb6f3e100ce524a2e44ce6c9aa850173510f8aab7a36ab26bf5a9c3c20
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6440e7eb6f3e100ce524a2e44ce6c9aa850173510f8aab7a36ab26bf5a9c3c20"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 46998bfb5281b01d99bf161a0ab57b1fa1098ba2525263a9183216ea1e37cdd7
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
      "id": 538,
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
      "created_at": "2016-10-19T11:45:26.487Z",
      "updated_at": "2016-10-19T11:45:26.487Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-19T11:45:26.564Z",
    "updated_at": "2016-10-19T11:45:26.564Z",
    "course_id": 176,
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
	-H "Authorization: Bearer 46998bfb5281b01d99bf161a0ab57b1fa1098ba2525263a9183216ea1e37cdd7"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/67/feedbacks
Content-Type: application/json
Authorization: Bearer b2a4d60218e36124c986a7e879e382d2b596fb3b0597544c30fb8f9e09f3f6f9
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
      "id": 46,
      "user_id": 849,
      "feedbackable_id": 67,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:47.262Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 848,
      "feedbackable_id": 67,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:47.249Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/67/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2a4d60218e36124c986a7e879e382d2b596fb3b0597544c30fb8f9e09f3f6f9"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer bbae010492e721e52847c8225750fcb72f296790257e101c3df87758486638a6
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
      "id": 38,
      "obfuscated_id": "8_YCqPYFnsI",
      "author_id": 642,
      "chapter_id": 143,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:35.494Z",
      "created_at": "2016-10-19T11:45:35.494Z",
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 645,
      "chapter_id": 144,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:35.637Z",
      "created_at": "2016-10-19T11:45:35.637Z",
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 648,
      "chapter_id": 145,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:35.778Z",
      "created_at": "2016-10-19T11:45:35.778Z",
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
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 651,
      "chapter_id": 146,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:35.918Z",
      "created_at": "2016-10-19T11:45:35.918Z",
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 654,
      "chapter_id": 147,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:36.055Z",
      "created_at": "2016-10-19T11:45:36.055Z",
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
	-H "Authorization: Bearer bbae010492e721e52847c8225750fcb72f296790257e101c3df87758486638a6"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 20580e87c2c0657dbcc2dc899122c8af6d7f0e6e733645efca0246bbc4b7aab5
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
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 670,
      "chapter_id": 152,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:36.819Z",
      "created_at": "2016-10-19T11:45:36.819Z",
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
	-H "Authorization: Bearer 20580e87c2c0657dbcc2dc899122c8af6d7f0e6e733645efca0246bbc4b7aab5"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/republish
Content-Type: application/json
Authorization: Bearer ef0195c7f5c3202555509bfc9385d15b065ef6cf18988ea452b8ebf75e171cc8
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef0195c7f5c3202555509bfc9385d15b065ef6cf18988ea452b8ebf75e171cc8"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/77/feedbacks
Content-Type: application/json
Authorization: Bearer 54c6f46187564e2cab84267be357165091c925db0ecd6e6e89023578ada5a298
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
      "id": 33,
      "user_id": 500,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:23.578Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 499,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:23.565Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/77/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54c6f46187564e2cab84267be357165091c925db0ecd6e6e89023578ada5a298"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 355c3279d2a94712c4707553814e0afebe85d727aec064446fc43b761357cc2f
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 88,
      "chapter_id": 24,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:49.771Z",
      "created_at": "2016-10-19T11:44:49.641Z",
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
          "id": 42,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 43,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 79,
      "chapter_id": 21,
      "position": 17,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:48.810Z",
      "created_at": "2016-10-19T11:44:48.684Z",
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
          "id": 36,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 37,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 82,
      "chapter_id": 22,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:49.123Z",
      "created_at": "2016-10-19T11:44:48.975Z",
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
          "id": 38,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 39,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 85,
      "chapter_id": 23,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:49.424Z",
      "created_at": "2016-10-19T11:44:49.295Z",
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
          "id": 40,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 41,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 91,
      "chapter_id": 25,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:50.090Z",
      "created_at": "2016-10-19T11:44:49.953Z",
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
          "id": 44,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 45,
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
	-H "Authorization: Bearer 355c3279d2a94712c4707553814e0afebe85d727aec064446fc43b761357cc2f"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 00ecf63d1e4993b8a17db600256e4da05a344dc27a0fde507d3d53dfa2b78a21
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
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 59,
      "chapter_id": 15,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:44:46.912Z",
      "created_at": "2016-10-19T11:44:46.794Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00ecf63d1e4993b8a17db600256e4da05a344dc27a0fde507d3d53dfa2b78a21"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/31/republish
Content-Type: application/json
Authorization: Bearer 0aa8c45be0274867336b2f63baa279d4d153f7ac21a86be09b9090e39882f93d
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aa8c45be0274867336b2f63baa279d4d153f7ac21a86be09b9090e39882f93d"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 326db18902451dc1b6f67b8b84fec7bbaaaa6a5dea55509c1ba923ed06f19fd9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":42,"published":false}}
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
    "creator_id": 127,
    "id": 42,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 43,
    "additional_university_ids": [

    ],
    "topic_id": 42,
    "discipline_id": 42,
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
    "updated_at": "2016-10-19T11:44:55.310Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":42,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 326db18902451dc1b6f67b8b84fec7bbaaaa6a5dea55509c1ba923ed06f19fd9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2774ad451554a53de2a984ccef96bc839c94074b03e266040e8911c6ceb488ce
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
      "creator_id": 159,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-54",
      "html_url": "https://goskive.com/course/fu-course-54",
      "slug": "fu-course-54",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 71,
      "discipline_id": 71,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 54",
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
      "updated_at": "2016-10-19T11:44:58.423Z",
      "shortname": "fu-course-54"
    },
    {
      "creator_id": 159,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-55",
      "html_url": "https://goskive.com/course/fu-course-55",
      "slug": "fu-course-55",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 72,
      "discipline_id": 72,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 55",
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
      "updated_at": "2016-10-19T11:44:58.465Z",
      "shortname": "fu-course-55"
    },
    {
      "creator_id": 160,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-56",
      "html_url": "https://goskive.com/course/fu-course-56",
      "slug": "fu-course-56",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 73,
      "discipline_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
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
      "updated_at": "2016-10-19T11:44:58.516Z",
      "shortname": "fu-course-56"
    },
    {
      "creator_id": 160,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
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
      "chapters_updated_at": "2016-10-19T11:44:58.821Z",
      "updated_at": "2016-10-19T11:44:58.827Z",
      "shortname": "fu-course-57"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2774ad451554a53de2a984ccef96bc839c94074b03e266040e8911c6ceb488ce"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 60ea748c5495c119a6d9fbf0ff7639caa51de9b380fee1fbe51738721f574e5e
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
      "creator_id": 166,
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
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
      "updated_at": "2016-10-19T11:44:59.038Z",
      "shortname": "fu-course-58"
    },
    {
      "creator_id": 166,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 76,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 59",
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
      "updated_at": "2016-10-19T11:44:59.079Z",
      "shortname": "fu-course-59"
    },
    {
      "creator_id": 167,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-60",
      "html_url": "https://goskive.com/course/fu-course-60",
      "slug": "fu-course-60",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 77,
      "discipline_id": 77,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 60",
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
      "updated_at": "2016-10-19T11:44:59.128Z",
      "shortname": "fu-course-60"
    },
    {
      "creator_id": 167,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-61",
      "html_url": "https://goskive.com/course/fu-course-61",
      "slug": "fu-course-61",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 78,
      "discipline_id": 78,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
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
      "updated_at": "2016-10-19T11:44:59.174Z",
      "shortname": "fu-course-61"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60ea748c5495c119a6d9fbf0ff7639caa51de9b380fee1fbe51738721f574e5e"
```
