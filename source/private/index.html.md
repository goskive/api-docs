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
DELETE /v2/chapters/72
Content-Type: application/json
Authorization: Bearer 3001a0335075d28cd8211285bba8f032977683087aa144551af95ac12abcd2a3
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/72" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3001a0335075d28cd8211285bba8f032977683087aa144551af95ac12abcd2a3"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/68
Content-Type: application/json
Authorization: Bearer ceef4c09584e4193e8ca54e4e1b0c08efb02b8fb156fac45133c982442946107
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
    "id": 68,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-29T17:22:14.672Z",
    "course_id": 86,
    "author_id": 316,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-29T17:22:14.122Z",
    "questions_updated_at": "2016-10-29T17:22:14.122Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 319,
        "chapter_id": 68,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:14.616Z",
        "created_at": "2016-10-29T17:22:14.616Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 320,
        "chapter_id": 68,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:14.653Z",
        "created_at": "2016-10-29T17:22:14.653Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 317,
        "chapter_id": 68,
        "position": 23,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:14.342Z",
        "created_at": "2016-10-29T17:22:14.224Z",
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
            "id": 45,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 46,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 318,
        "chapter_id": 68,
        "position": 24,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:14.545Z",
        "created_at": "2016-10-29T17:22:14.416Z",
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
            "id": 47,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 48,
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
curl "api.goskive.com/v2/chapters/68" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceef4c09584e4193e8ca54e4e1b0c08efb02b8fb156fac45133c982442946107"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/66
Content-Type: application/json
Authorization: Bearer d1c4f67ce9011f4528c4360f06df1ba66c2b01293dc620ceaef202cca7f5498a
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
    "id": 66,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-29T17:22:13.973Z",
    "course_id": 84,
    "author_id": 310,
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
curl "api.goskive.com/v2/chapters/66" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1c4f67ce9011f4528c4360f06df1ba66c2b01293dc620ceaef202cca7f5498a"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 6ce73b7c5341cc950e12397b9bfa279665c428cb5b42178fcf500745c1bb5343
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ce73b7c5341cc950e12397b9bfa279665c428cb5b42178fcf500745c1bb5343"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d7d330ba7834f7c55cbe210e4e9cca61898f4f51786de9ac3cc25d447002f94c
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
      "id": 19,
      "author_id": 370,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:17.685Z",
      "status": "published",
      "subject_id": 104,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 372,
      "reply_to_id": 19,
      "created_at": "2016-10-29T17:22:17.771Z",
      "status": "published",
      "subject_id": 105,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 374,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:17.852Z",
      "status": "published",
      "subject_id": 106,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 376,
      "reply_to_id": 21,
      "created_at": "2016-10-29T17:22:17.932Z",
      "status": "published",
      "subject_id": 107,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 378,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:18.013Z",
      "status": "reported",
      "subject_id": 108,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 380,
      "reply_to_id": 23,
      "created_at": "2016-10-29T17:22:18.092Z",
      "status": "published",
      "subject_id": 109,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 382,
      "reply_to_id": 23,
      "created_at": "2016-10-29T17:22:18.171Z",
      "status": "published",
      "subject_id": 110,
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
	-H "Authorization: Bearer d7d330ba7834f7c55cbe210e4e9cca61898f4f51786de9ac3cc25d447002f94c"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer b80c1878016cec422304c317194b55dc0b8f3462a0e791837deb3bae4aac5d29
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
      "id": 33,
      "author_id": 400,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:18.911Z",
      "status": "published",
      "subject_id": 118,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 402,
      "reply_to_id": 33,
      "created_at": "2016-10-29T17:22:18.995Z",
      "status": "published",
      "subject_id": 119,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 404,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:19.078Z",
      "status": "published",
      "subject_id": 120,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 406,
      "reply_to_id": 35,
      "created_at": "2016-10-29T17:22:19.190Z",
      "status": "published",
      "subject_id": 121,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 408,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:19.269Z",
      "status": "reported",
      "subject_id": 122,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 410,
      "reply_to_id": 37,
      "created_at": "2016-10-29T17:22:19.348Z",
      "status": "published",
      "subject_id": 123,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 412,
      "reply_to_id": 37,
      "created_at": "2016-10-29T17:22:19.428Z",
      "status": "published",
      "subject_id": 124,
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
	-H "Authorization: Bearer b80c1878016cec422304c317194b55dc0b8f3462a0e791837deb3bae4aac5d29"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 3573b3d47028411d1ac0e6b65b9aeccdbd6069b6e7c15b744e0806731fa02ca3
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
      "id": 13,
      "author_id": 357,
      "reply_to_id": 12,
      "created_at": "2016-10-29T17:22:17.146Z",
      "status": "published",
      "subject_id": 98,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 361,
      "reply_to_id": 14,
      "created_at": "2016-10-29T17:22:17.305Z",
      "status": "published",
      "subject_id": 100,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 365,
      "reply_to_id": 16,
      "created_at": "2016-10-29T17:22:17.465Z",
      "status": "published",
      "subject_id": 102,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 367,
      "reply_to_id": 16,
      "created_at": "2016-10-29T17:22:17.544Z",
      "status": "published",
      "subject_id": 103,
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
	-H "Authorization: Bearer 3573b3d47028411d1ac0e6b65b9aeccdbd6069b6e7c15b744e0806731fa02ca3"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 9224e0df9c1be4206a1954162693cb662d52543c27523e421f9be543cd44dabf
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
      "id": 44,
      "author_id": 423,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:19.880Z",
      "status": "reported",
      "subject_id": 129,
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
	-H "Authorization: Bearer 9224e0df9c1be4206a1954162693cb662d52543c27523e421f9be543cd44dabf"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/11/republish
Content-Type: application/json
Authorization: Bearer 375b16410ee31d35be3b7bb84c3828dad559a6ffaa3a4b0d26f730a1a8e3f776
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 375b16410ee31d35be3b7bb84c3828dad559a6ffaa3a4b0d26f730a1a8e3f776"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2d6a48417c71644f706e5626d66b69f374e61b65b8b8a5cf4e5ab6f38139bbc6
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
    "id": 167,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-29T17:23:06.663Z",
    "course_id": 291,
    "author_id": 900,
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
	-H "Authorization: Bearer 2d6a48417c71644f706e5626d66b69f374e61b65b8b8a5cf4e5ab6f38139bbc6"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/293/chapters
Content-Type: application/json
Authorization: Bearer e8eaafa64ccbf9ba435c9542f3ea2f7670d02d0971d56a340c3c96e29eef6f68
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
    "updated_at": "2016-10-29T17:23:06.918Z",
    "course_id": 293,
    "author_id": 904,
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
curl "api.goskive.com/v2/courses/293/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8eaafa64ccbf9ba435c9542f3ea2f7670d02d0971d56a340c3c96e29eef6f68"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 57a60c670be6f6277c0e118a72e53a3a2890e2e2beef71071a90a93bdcff4a8f
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
      "id": 185,
      "title": "Clever Chapter Title 161",
      "position": 1,
      "updated_at": "2016-10-29T17:23:08.652Z",
      "course_id": 302,
      "author_id": 938,
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
      "position": 2,
      "updated_at": "2016-10-29T17:23:08.675Z",
      "course_id": 302,
      "author_id": 939,
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
      "id": 187,
      "title": "Clever Chapter Title 163",
      "position": 3,
      "updated_at": "2016-10-29T17:23:08.919Z",
      "course_id": 302,
      "author_id": 940,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-29T17:23:08.579Z",
      "questions_updated_at": "2016-10-29T17:23:08.579Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57a60c670be6f6277c0e118a72e53a3a2890e2e2beef71071a90a93bdcff4a8f"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 811863fbb0625ff818a9860cc8d64844be8ef8f9ecf0e5914168bee6106b97b9
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
      "id": 188,
      "title": "Clever Chapter Title 164",
      "position": 1,
      "updated_at": "2016-10-29T17:23:09.061Z",
      "course_id": 303,
      "author_id": 945,
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
      "position": 2,
      "updated_at": "2016-10-29T17:23:09.085Z",
      "course_id": 303,
      "author_id": 946,
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
      "id": 190,
      "title": "Clever Chapter Title 166",
      "position": 3,
      "updated_at": "2016-10-29T17:23:09.108Z",
      "course_id": 303,
      "author_id": 947,
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
	-H "Authorization: Bearer 811863fbb0625ff818a9860cc8d64844be8ef8f9ecf0e5914168bee6106b97b9"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/187
Content-Type: application/json
Authorization: Bearer 134d7607307e0a5376c8f360e4d5aacec36320b5fc2c68e13005636820bc8949
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/187" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 134d7607307e0a5376c8f360e4d5aacec36320b5fc2c68e13005636820bc8949"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 408e7f32008d7ec8467966124f0063e5afd0b8dafc9e1ea16a495252378df753
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
	-H "Authorization: Bearer 408e7f32008d7ec8467966124f0063e5afd0b8dafc9e1ea16a495252378df753"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 57253505ca535ecaed5d69f025c4c316cff7942bc6696950f77f5f8156d22ad4
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
    "creator_id": 512,
    "id": 181,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 159,
    "additional_university_ids": [

    ],
    "topic_id": 191,
    "discipline_id": 192,
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
    "chapters_updated_at": "2016-10-29T17:22:30.606Z",
    "updated_at": "2016-10-29T17:22:32.260Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 90,
        "title": "Clever Chapter Title 78",
        "position": 1,
        "updated_at": "2016-10-29T17:22:32.209Z",
        "course_id": 181,
        "author_id": 512,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-29T17:22:30.606Z",
        "questions_updated_at": "2016-10-29T17:22:30.606Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 91,
        "title": "Clever Chapter Title 79",
        "position": 2,
        "updated_at": "2016-10-29T17:22:32.251Z",
        "course_id": 181,
        "author_id": 512,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-29T17:22:30.606Z",
        "questions_updated_at": "2016-10-29T17:22:30.606Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 512,
        "chapter_id": 90,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.034Z",
        "created_at": "2016-10-29T17:22:32.034Z",
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
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 512,
        "chapter_id": 91,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.110Z",
        "created_at": "2016-10-29T17:22:32.110Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 512,
        "chapter_id": 90,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.077Z",
        "created_at": "2016-10-29T17:22:32.077Z",
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
        "id": 66,
        "obfuscated_id": "H7dODBospvw",
        "author_id": 512,
        "chapter_id": 91,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.155Z",
        "created_at": "2016-10-29T17:22:32.155Z",
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
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 515,
        "chapter_id": 90,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.197Z",
        "created_at": "2016-10-29T17:22:32.197Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 516,
        "chapter_id": 91,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:32.239Z",
        "created_at": "2016-10-29T17:22:32.239Z",
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
	-H "Authorization: Bearer 57253505ca535ecaed5d69f025c4c316cff7942bc6696950f77f5f8156d22ad4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/186
Content-Type: application/json
Authorization: Bearer 0c7ec51e6fb3535ab988bc8559553d7f4538a941b7570ab2f59b9b5ac8925915
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
    "creator_id": 529,
    "id": 186,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "topic_id": 196,
    "discipline_id": 197,
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
    "updated_at": "2016-10-29T17:22:34.744Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/186" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c7ec51e6fb3535ab988bc8559553d7f4538a941b7570ab2f59b9b5ac8925915"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 060bbaab7aae44bfe142290c0fb2df8891df37c006c6a0faa18456df4fa111a1
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
    "creator_id": 527,
    "id": 185,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "topic_id": 195,
    "discipline_id": 196,
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
    "updated_at": "2016-10-29T17:22:34.594Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 060bbaab7aae44bfe142290c0fb2df8891df37c006c6a0faa18456df4fa111a1"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer a5860449b2c762c28d81d712b781718c1a6f6b49c449ddda7212107b437ea56a
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
      "user_id": 193,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:06.585Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 197,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:06.861Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 201,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:07.140Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 205,
      "feedbackable_id": 7,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:07.415Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 209,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-29T17:22:07.693Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5860449b2c762c28d81d712b781718c1a6f6b49c449ddda7212107b437ea56a"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer e4b5fa2557ad8d144ec40b00e0efc8728656caa35e1bfc7a683c4a98e883976e
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
      "id": 28,
      "user_id": 267,
      "feedbackable_id": 22,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-29T17:22:11.859Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4b5fa2557ad8d144ec40b00e0efc8728656caa35e1bfc7a683c4a98e883976e"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer f828df9d2e79bec44f241519eedc50b45582a9cd40bfdd1033ccd241f87c6fc6
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f828df9d2e79bec44f241519eedc50b45582a9cd40bfdd1033ccd241f87c6fc6"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer 4dbc9345b77087693fd483bdbe89e1b25832f255c4961f3a321e45c55ba3828b
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
    "id": 12,
    "uploader": {
      "id": 582,
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
      "created_at": "2016-10-29T17:22:38.141Z",
      "updated_at": "2016-10-29T17:22:38.141Z"
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
    "created_at": "2016-10-29T17:22:38.212Z",
    "updated_at": "2016-10-29T17:22:38.212Z",
    "course_id": 206,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4dbc9345b77087693fd483bdbe89e1b25832f255c4961f3a321e45c55ba3828b"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/37/feedbacks
Content-Type: application/json
Authorization: Bearer 4af19a84a12d649687f3b095073635115c6323014ee44b846bd28e5b9a717d98
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
      "id": 32,
      "user_id": 283,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:12.449Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 282,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:12.438Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/37/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4af19a84a12d649687f3b095073635115c6323014ee44b846bd28e5b9a717d98"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer f4610ea788a2cca145b3500d696bf5be6267213bff68fe798d65bcabb7d5e56b
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 36,
      "chapter_id": 11,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:56.448Z",
      "created_at": "2016-10-29T17:21:56.448Z",
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
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 39,
      "chapter_id": 12,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:56.564Z",
      "created_at": "2016-10-29T17:21:56.564Z",
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 42,
      "chapter_id": 13,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:56.682Z",
      "created_at": "2016-10-29T17:21:56.682Z",
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 45,
      "chapter_id": 14,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:56.800Z",
      "created_at": "2016-10-29T17:21:56.800Z",
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 48,
      "chapter_id": 15,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:56.917Z",
      "created_at": "2016-10-29T17:21:56.917Z",
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
	-H "Authorization: Bearer f4610ea788a2cca145b3500d696bf5be6267213bff68fe798d65bcabb7d5e56b"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 207b78213eff21eeb1580ea2ab6d8208b209ef9fc4ece49d23d23db4e3272cbc
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
      "id": 5,
      "obfuscated_id": "iw-7peoPwEU",
      "author_id": 16,
      "chapter_id": 5,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:21:55.665Z",
      "created_at": "2016-10-29T17:21:55.665Z",
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
	-H "Authorization: Bearer 207b78213eff21eeb1580ea2ab6d8208b209ef9fc4ece49d23d23db4e3272cbc"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/republish
Content-Type: application/json
Authorization: Bearer a7d89702a81695eec994b90b900fac5b94da68fe295e92ccb84a602ef697e4ac
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7d89702a81695eec994b90b900fac5b94da68fe295e92ccb84a602ef697e4ac"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/116/feedbacks
Content-Type: application/json
Authorization: Bearer 618fe043c6fc269b0207b3d0bace4190893fe25f283edeb7506e5935924f78b9
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
      "user_id": 821,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:59.709Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 820,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:59.699Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/116/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 618fe043c6fc269b0207b3d0bace4190893fe25f283edeb7506e5935924f78b9"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 5e965aafc9f49be5a8eccaef25ba2ede249afefdde3a98a2d580a8746bbe2c10
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 628,
      "chapter_id": 110,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:42.469Z",
      "created_at": "2016-10-29T17:22:42.358Z",
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
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 637,
      "chapter_id": 113,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:43.297Z",
      "created_at": "2016-10-29T17:22:43.176Z",
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
      "author_id": 631,
      "chapter_id": 111,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:42.737Z",
      "created_at": "2016-10-29T17:22:42.622Z",
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
      "author_id": 634,
      "chapter_id": 112,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:43.013Z",
      "created_at": "2016-10-29T17:22:42.897Z",
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
      "author_id": 640,
      "chapter_id": 114,
      "position": 68,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:43.595Z",
      "created_at": "2016-10-29T17:22:43.486Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e965aafc9f49be5a8eccaef25ba2ede249afefdde3a98a2d580a8746bbe2c10"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 500e6eda5aba4a06a3c93aab7cd0b50cb4953bd43e36ee0df151acc75041db6d
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
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 672,
      "chapter_id": 124,
      "position": 78,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:46.431Z",
      "created_at": "2016-10-29T17:22:46.321Z",
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
          "id": 170,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 171,
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
	-H "Authorization: Bearer 500e6eda5aba4a06a3c93aab7cd0b50cb4953bd43e36ee0df151acc75041db6d"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/87/republish
Content-Type: application/json
Authorization: Bearer aab3c637acc15cd887dfc507cf6e36e8141cf0e35c5c217e5ea6bea10693cd90
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/87/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aab3c637acc15cd887dfc507cf6e36e8141cf0e35c5c217e5ea6bea10693cd90"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2d47fcd6174fb89353d0e10e1fb583b3f758c5e64b15342ce2a61aafdd7e7af8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":149,"published":false}}
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
    "creator_id": 455,
    "id": 139,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 139,
    "additional_university_ids": [

    ],
    "topic_id": 149,
    "discipline_id": 150,
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
    "updated_at": "2016-10-29T17:22:22.897Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":149,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d47fcd6174fb89353d0e10e1fb583b3f758c5e64b15342ce2a61aafdd7e7af8"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 095a0e0bd8c084ec17cffdd558911f8b735e1a7ba22ef8d39d439495fd53fb5c
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
      "creator_id": 489,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
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
      "updated_at": "2016-10-29T17:22:26.166Z",
      "shortname": "fu-course-147"
    },
    {
      "creator_id": 489,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
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
      "updated_at": "2016-10-29T17:22:26.205Z",
      "shortname": "fu-course-148"
    },
    {
      "creator_id": 490,
      "id": 172,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 183,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
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
      "updated_at": "2016-10-29T17:22:26.252Z",
      "shortname": "fu-course-149"
    },
    {
      "creator_id": 490,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 183,
      "discipline_id": 184,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
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
      "chapters_updated_at": "2016-10-29T17:22:26.573Z",
      "updated_at": "2016-10-29T17:22:26.581Z",
      "shortname": "fu-course-150"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 095a0e0bd8c084ec17cffdd558911f8b735e1a7ba22ef8d39d439495fd53fb5c"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 357ac45ada38cec19c5b3e061b9e64ad32a9352b75450c59a2c3b4f7158f3848
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
      "creator_id": 496,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 184,
      "discipline_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
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
      "updated_at": "2016-10-29T17:22:26.775Z",
      "shortname": "fu-course-151"
    },
    {
      "creator_id": 496,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
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
      "updated_at": "2016-10-29T17:22:26.814Z",
      "shortname": "fu-course-152"
    },
    {
      "creator_id": 497,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 186,
      "discipline_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 153",
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
      "updated_at": "2016-10-29T17:22:26.860Z",
      "shortname": "fu-course-153"
    },
    {
      "creator_id": 497,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-154",
      "html_url": "https://goskive.com/course/fu-course-154",
      "slug": "fu-course-154",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 187,
      "discipline_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 154",
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
      "updated_at": "2016-10-29T17:22:26.898Z",
      "shortname": "fu-course-154"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 357ac45ada38cec19c5b3e061b9e64ad32a9352b75450c59a2c3b4f7158f3848"
```
