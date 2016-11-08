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
DELETE /v2/chapters/23
Content-Type: application/json
Authorization: Bearer 27f39e07d70ebad540fa504b4271eb3fef383209655045c242f8935b0176ab86
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27f39e07d70ebad540fa504b4271eb3fef383209655045c242f8935b0176ab86"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/28
Content-Type: application/json
Authorization: Bearer 52bf81142c8904175c18cbb6c20e030206eda39ecc5fcda8054268fcc8dee1d7
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
    "id": 28,
    "updated_at": "2016-11-08T14:21:07.763Z",
    "course_id": 42,
    "author_id": 146,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-08T14:21:07.239Z",
    "questions_updated_at": "2016-11-08T14:21:07.239Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 149,
        "chapter_id": 28,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.708Z",
        "created_at": "2016-11-08T14:21:07.708Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 150,
        "chapter_id": 28,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.745Z",
        "created_at": "2016-11-08T14:21:07.745Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 147,
        "chapter_id": 28,
        "position": 10,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.449Z",
        "created_at": "2016-11-08T14:21:07.338Z",
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
            "id": 19,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 20,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 148,
        "chapter_id": 28,
        "position": 11,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.640Z",
        "created_at": "2016-11-08T14:21:07.518Z",
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
            "id": 21,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 22,
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
curl "api.goskive.com/v2/chapters/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52bf81142c8904175c18cbb6c20e030206eda39ecc5fcda8054268fcc8dee1d7"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/20
Content-Type: application/json
Authorization: Bearer 548c605ba9f346fa93b210c209692d3e1fa3a53050e381f99c781f344c5ab767
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
    "id": 20,
    "updated_at": "2016-11-08T14:21:05.153Z",
    "course_id": 34,
    "author_id": 119,
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
curl "api.goskive.com/v2/chapters/20" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 548c605ba9f346fa93b210c209692d3e1fa3a53050e381f99c781f344c5ab767"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/56
Content-Type: application/json
Authorization: Bearer ea642a644013979a2be8735b78e02de754295b37cfae830736c259040f3dc4c6
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea642a644013979a2be8735b78e02de754295b37cfae830736c259040f3dc4c6"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer baa463849f5b2328ccc94fbcda8092bf53ec27208029af7b50c6f37cdcc6bcb3
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
      "author_id": 530,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:38.736Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 532,
      "reply_to_id": 33,
      "created_at": "2016-11-08T14:21:38.819Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 534,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:38.906Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 536,
      "reply_to_id": 35,
      "created_at": "2016-11-08T14:21:38.988Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 538,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:39.069Z",
      "status": "reported",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 540,
      "reply_to_id": 37,
      "created_at": "2016-11-08T14:21:39.149Z",
      "status": "published",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 542,
      "reply_to_id": 37,
      "created_at": "2016-11-08T14:21:39.230Z",
      "status": "published",
      "subject_id": 162,
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
	-H "Authorization: Bearer baa463849f5b2328ccc94fbcda8092bf53ec27208029af7b50c6f37cdcc6bcb3"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 1b069695d04082371dc488080dcc13a31d6efbc1262a2258617c9ffd751963a4
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
      "id": 40,
      "author_id": 545,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:39.372Z",
      "status": "published",
      "subject_id": 163,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 547,
      "reply_to_id": 40,
      "created_at": "2016-11-08T14:21:39.453Z",
      "status": "published",
      "subject_id": 164,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 549,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:39.536Z",
      "status": "published",
      "subject_id": 165,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 551,
      "reply_to_id": 42,
      "created_at": "2016-11-08T14:21:39.615Z",
      "status": "published",
      "subject_id": 166,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 553,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:39.699Z",
      "status": "reported",
      "subject_id": 167,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 555,
      "reply_to_id": 44,
      "created_at": "2016-11-08T14:21:39.780Z",
      "status": "published",
      "subject_id": 168,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 557,
      "reply_to_id": 44,
      "created_at": "2016-11-08T14:21:39.860Z",
      "status": "published",
      "subject_id": 169,
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
	-H "Authorization: Bearer 1b069695d04082371dc488080dcc13a31d6efbc1262a2258617c9ffd751963a4"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer c8410f8fc1e79dbd073c6742fbd854aefdd077422fa5432651a87c7a4f643d69
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
      "id": 20,
      "author_id": 502,
      "reply_to_id": 19,
      "created_at": "2016-11-08T14:21:37.562Z",
      "status": "published",
      "subject_id": 143,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 506,
      "reply_to_id": 21,
      "created_at": "2016-11-08T14:21:37.726Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 510,
      "reply_to_id": 23,
      "created_at": "2016-11-08T14:21:37.921Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 512,
      "reply_to_id": 23,
      "created_at": "2016-11-08T14:21:38.002Z",
      "status": "published",
      "subject_id": 148,
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
	-H "Authorization: Bearer c8410f8fc1e79dbd073c6742fbd854aefdd077422fa5432651a87c7a4f643d69"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 344d20c6cd497efb369f5781dc42f0eedac26b7308e607d946471c007e27e280
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
      "id": 30,
      "author_id": 523,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:38.451Z",
      "status": "reported",
      "subject_id": 153,
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
	-H "Authorization: Bearer 344d20c6cd497efb369f5781dc42f0eedac26b7308e607d946471c007e27e280"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/18/republish
Content-Type: application/json
Authorization: Bearer 49c73f667912c175ea8df5faa1e7434909a40c12312a3b414cbca06d3cebd6cc
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/18/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49c73f667912c175ea8df5faa1e7434909a40c12312a3b414cbca06d3cebd6cc"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4015aa3cf780fe8cbce08b2b5ba8799878d76c51e990dc631589f0cc63c81340
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
    "id": 50,
    "updated_at": "2016-11-08T14:21:10.654Z",
    "course_id": 56,
    "author_id": 203,
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
	-H "Authorization: Bearer 4015aa3cf780fe8cbce08b2b5ba8799878d76c51e990dc631589f0cc63c81340"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/59/chapters
Content-Type: application/json
Authorization: Bearer 6c19ee928d40865b6dcd407c792fa90fff987a488f151e5205eb3035aca2acba
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
    "id": 52,
    "updated_at": "2016-11-08T14:21:11.122Z",
    "course_id": 59,
    "author_id": 209,
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
curl "api.goskive.com/v2/courses/59/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c19ee928d40865b6dcd407c792fa90fff987a488f151e5205eb3035aca2acba"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer bff3b6807506e186fc3249e4a1630ae6ad2483d9b7df74ff787d562847ba9993
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
      "id": 32,
      "updated_at": "2016-11-08T14:21:08.589Z",
      "course_id": 47,
      "author_id": 164,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 23",
      "position": 1
    },
    {
      "id": 33,
      "updated_at": "2016-11-08T14:21:08.611Z",
      "course_id": 47,
      "author_id": 165,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 24",
      "position": 2
    },
    {
      "id": 34,
      "updated_at": "2016-11-08T14:21:08.860Z",
      "course_id": 47,
      "author_id": 166,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-08T14:21:08.521Z",
      "questions_updated_at": "2016-11-08T14:21:08.521Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 25",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bff3b6807506e186fc3249e4a1630ae6ad2483d9b7df74ff787d562847ba9993"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 90e51d66c3f131979dcd3f58aeea9d73c20e6f89293cf71ffee9dce716fc5c38
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
      "id": 35,
      "updated_at": "2016-11-08T14:21:09.097Z",
      "course_id": 49,
      "author_id": 173,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 26",
      "position": 1
    },
    {
      "id": 36,
      "updated_at": "2016-11-08T14:21:09.120Z",
      "course_id": 49,
      "author_id": 174,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 27",
      "position": 2
    },
    {
      "id": 37,
      "updated_at": "2016-11-08T14:21:09.142Z",
      "course_id": 49,
      "author_id": 175,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 28",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90e51d66c3f131979dcd3f58aeea9d73c20e6f89293cf71ffee9dce716fc5c38"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/303
Content-Type: application/json
Authorization: Bearer 8ffe32db30a535dd79c5c7169e2ca569d7aa92b2a70aec0dc3d637c1c8208e0c
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/303" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ffe32db30a535dd79c5c7169e2ca569d7aa92b2a70aec0dc3d637c1c8208e0c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 91028a64fdf0c3c6634e808c13eb4236ee9f5caa3a015c9960ce10dc7216429a
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
	-H "Authorization: Bearer 91028a64fdf0c3c6634e808c13eb4236ee9f5caa3a015c9960ce10dc7216429a"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 37a1400a609ac56447fb270a3feaa6e9d1e27adbfc83a35f5761c05db42a6ec5
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
    "creator_id": 974,
    "id": 315,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 299,
    "additional_university_ids": [

    ],
    "discipline_id": 326,
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
    "chapters_updated_at": "2016-11-08T14:22:15.957Z",
    "updated_at": "2016-11-08T14:22:17.367Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 974,
        "chapter_id": 194,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.144Z",
        "created_at": "2016-11-08T14:22:17.144Z",
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
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 974,
        "chapter_id": 195,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.221Z",
        "created_at": "2016-11-08T14:22:17.221Z",
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
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 974,
        "chapter_id": 194,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.186Z",
        "created_at": "2016-11-08T14:22:17.186Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 974,
        "chapter_id": 195,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.264Z",
        "created_at": "2016-11-08T14:22:17.264Z",
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
        "id": 94,
        "obfuscated_id": "CVi6VU_nV6k",
        "author_id": 977,
        "chapter_id": 194,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.306Z",
        "created_at": "2016-11-08T14:22:17.306Z",
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
        "author_id": 978,
        "chapter_id": 195,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:17.348Z",
        "created_at": "2016-11-08T14:22:17.348Z",
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
        "id": 194,
        "updated_at": "2016-11-08T14:22:17.317Z",
        "course_id": 315,
        "author_id": 974,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-08T14:22:15.957Z",
        "questions_updated_at": "2016-11-08T14:22:15.957Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 170",
        "position": 1
      },
      {
        "id": 195,
        "updated_at": "2016-11-08T14:22:17.358Z",
        "course_id": 315,
        "author_id": 974,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-08T14:22:15.957Z",
        "questions_updated_at": "2016-11-08T14:22:15.957Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 171",
        "position": 2
      }
    ],
    "topic_id": 325,
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
	-H "Authorization: Bearer 37a1400a609ac56447fb270a3feaa6e9d1e27adbfc83a35f5761c05db42a6ec5"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/301
Content-Type: application/json
Authorization: Bearer 3481d0481842530109b0edaea6ad64c34652740ed1220b2f7bbc8a957967f16f
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
    "creator_id": 933,
    "id": 301,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 285,
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
    "updated_at": "2016-11-08T14:22:09.770Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 311,
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
curl "api.goskive.com/v2/courses/301" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3481d0481842530109b0edaea6ad64c34652740ed1220b2f7bbc8a957967f16f"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer aacfc79c8c6ff7dd889c0fae73a1120b515b070a3800fbea1246306f1121e97c
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
    "creator_id": 928,
    "id": 298,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 282,
    "additional_university_ids": [

    ],
    "discipline_id": 309,
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
    "updated_at": "2016-11-08T14:22:09.364Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 308,
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
	-H "Authorization: Bearer aacfc79c8c6ff7dd889c0fae73a1120b515b070a3800fbea1246306f1121e97c"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer f92b2781947a2157ec53c78be3b721d6819af96c08805530586ed3fc6f87f89d
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
      "id": 35,
      "user_id": 698,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:49.069Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 702,
      "feedbackable_id": 80,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:49.351Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 37,
      "user_id": 706,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:49.636Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 38,
      "user_id": 710,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:49.930Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 714,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-08T14:21:50.217Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f92b2781947a2157ec53c78be3b721d6819af96c08805530586ed3fc6f87f89d"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 5022f505d2c28c713fdc1d82bc82ab1eb22806488264afd0f9d16e0da37bdd08
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
      "id": 25,
      "user_id": 656,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-08T14:21:46.044Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5022f505d2c28c713fdc1d82bc82ab1eb22806488264afd0f9d16e0da37bdd08"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 92badaaeb4c7297cd1277b1209bf519f98edb71d614267943afe3157926594fd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92badaaeb4c7297cd1277b1209bf519f98edb71d614267943afe3157926594fd"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/17/metadata
Content-Type: application/json
Authorization: Bearer b4312fd3767c6a9b465754fb79c63854f485cae6863bf2363a99d4af1f369f8f
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
    "id": 17,
    "uploader": {
      "id": 911,
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
      "created_at": "2016-11-08T14:22:08.487Z",
      "updated_at": "2016-11-08T14:22:08.487Z"
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
    "created_at": "2016-11-08T14:22:08.559Z",
    "updated_at": "2016-11-08T14:22:08.559Z",
    "course_id": 292,
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
curl "api.goskive.com/v2/files/17/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4312fd3767c6a9b465754fb79c63854f485cae6863bf2363a99d4af1f369f8f"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/3/feedbacks
Content-Type: application/json
Authorization: Bearer 54e42a7b9efa33d434e143933eaa8b8a6eb9e0fca8aa3768ac3f4501c1d463e0
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
      "id": 3,
      "user_id": 66,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:02.087Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 65,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:02.076Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54e42a7b9efa33d434e143933eaa8b8a6eb9e0fca8aa3768ac3f4501c1d463e0"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 885ff2c914a9a5b95f8a29b298f6caac8c6fcd1d74f1649dd69c9d010588cb41
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
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 258,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:14.622Z",
      "created_at": "2016-11-08T14:21:14.622Z",
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 261,
      "chapter_id": 65,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:14.777Z",
      "created_at": "2016-11-08T14:21:14.777Z",
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
      "author_id": 264,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:14.908Z",
      "created_at": "2016-11-08T14:21:14.908Z",
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
      "author_id": 267,
      "chapter_id": 67,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:15.036Z",
      "created_at": "2016-11-08T14:21:15.036Z",
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
      "author_id": 270,
      "chapter_id": 68,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:15.166Z",
      "created_at": "2016-11-08T14:21:15.166Z",
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
	-H "Authorization: Bearer 885ff2c914a9a5b95f8a29b298f6caac8c6fcd1d74f1649dd69c9d010588cb41"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer dc26c03a7b28b06e10d15b199d1e99186285df053ef5ffc1eb5ddd3084a8ffaf
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 254,
      "chapter_id": 63,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:14.466Z",
      "created_at": "2016-11-08T14:21:14.466Z",
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
	-H "Authorization: Bearer dc26c03a7b28b06e10d15b199d1e99186285df053ef5ffc1eb5ddd3084a8ffaf"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/22/republish
Content-Type: application/json
Authorization: Bearer 6c5f2d6310742adb4341ea265bb7844167614b65e071f71183035a395cad1212
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/22/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c5f2d6310742adb4341ea265bb7844167614b65e071f71183035a395cad1212"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/60/feedbacks
Content-Type: application/json
Authorization: Bearer 42a9d0320fba0430d28f46ddbbbdcad8710a498d7c0ca3c68d027b0d212f0c38
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
      "id": 18,
      "user_id": 486,
      "feedbackable_id": 60,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:36.661Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 485,
      "feedbackable_id": 60,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:36.650Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/60/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42a9d0320fba0430d28f46ddbbbdcad8710a498d7c0ca3c68d027b0d212f0c38"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer e960e1ba2fc75adbc8554494dc2c7c9895d714848d4aabd40465322c9eaf6924
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 376,
      "chapter_id": 99,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:25.222Z",
      "created_at": "2016-11-08T14:21:25.078Z",
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
          "id": 68,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 69,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 367,
      "chapter_id": 96,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:24.284Z",
      "created_at": "2016-11-08T14:21:24.148Z",
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
          "id": 62,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 63,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 370,
      "chapter_id": 97,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:24.593Z",
      "created_at": "2016-11-08T14:21:24.450Z",
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
          "id": 64,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 65,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 373,
      "chapter_id": 98,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:24.908Z",
      "created_at": "2016-11-08T14:21:24.764Z",
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
          "id": 66,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 67,
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
      "author_id": 379,
      "chapter_id": 100,
      "position": 26,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:25.540Z",
      "created_at": "2016-11-08T14:21:25.396Z",
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
          "id": 70,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 71,
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
	-H "Authorization: Bearer e960e1ba2fc75adbc8554494dc2c7c9895d714848d4aabd40465322c9eaf6924"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer a986273bffa10204c1e47eeff201e758cbec7959d9f9921814e45493007f6cda
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 395,
      "chapter_id": 105,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:27.223Z",
      "created_at": "2016-11-08T14:21:27.055Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a986273bffa10204c1e47eeff201e758cbec7959d9f9921814e45493007f6cda"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/29/republish
Content-Type: application/json
Authorization: Bearer 6e819c9869cc0f8d02560e5d4782e937c9999c928a743c28b5a0ac7c1c28df36
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/29/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e819c9869cc0f8d02560e5d4782e937c9999c928a743c28b5a0ac7c1c28df36"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer da0c8b0252aa5bd313e6830a03c266eeea77359d03632c278bb18be6b08c0c7a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":293,"published":false}}
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
    "creator_id": 880,
    "id": 283,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 267,
    "additional_university_ids": [

    ],
    "discipline_id": 294,
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
    "updated_at": "2016-11-08T14:22:05.262Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 293,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":293,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da0c8b0252aa5bd313e6830a03c266eeea77359d03632c278bb18be6b08c0c7a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4d5c679d6344ffe2a7a9333c8637104745bf3761f6e1dd019e66a2e38b19cff1
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
      "creator_id": 841,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 260,
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
      "updated_at": "2016-11-08T14:22:01.559Z",
      "shortname": "fu-course-196",
      "topic_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 841,
      "id": 250,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-197",
      "html_url": "https://goskive.com/course/fu-course-197",
      "slug": "fu-course-197",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 261,
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
      "updated_at": "2016-11-08T14:22:01.597Z",
      "shortname": "fu-course-197",
      "topic_id": 260,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 197",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 842,
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-198",
      "html_url": "https://goskive.com/course/fu-course-198",
      "slug": "fu-course-198",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 262,
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
      "updated_at": "2016-11-08T14:22:01.642Z",
      "shortname": "fu-course-198",
      "topic_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 198",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 842,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 263,
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
      "chapters_updated_at": "2016-11-08T14:22:01.501Z",
      "updated_at": "2016-11-08T14:22:01.939Z",
      "shortname": "fu-course-199",
      "topic_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d5c679d6344ffe2a7a9333c8637104745bf3761f6e1dd019e66a2e38b19cff1"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2bb1ce90b332e548dc1ce629ba8a3d2b31636ca983790ee49d4966ad14213cbb
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
      "creator_id": 848,
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-200",
      "html_url": "https://goskive.com/course/fu-course-200",
      "slug": "fu-course-200",
      "university_id": 255,
      "additional_university_ids": [

      ],
      "discipline_id": 264,
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
      "updated_at": "2016-11-08T14:22:02.138Z",
      "shortname": "fu-course-200",
      "topic_id": 263,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 200",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 848,
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-201",
      "html_url": "https://goskive.com/course/fu-course-201",
      "slug": "fu-course-201",
      "university_id": 255,
      "additional_university_ids": [

      ],
      "discipline_id": 265,
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
      "updated_at": "2016-11-08T14:22:02.177Z",
      "shortname": "fu-course-201",
      "topic_id": 264,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 201",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 849,
      "id": 255,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-202",
      "html_url": "https://goskive.com/course/fu-course-202",
      "slug": "fu-course-202",
      "university_id": 255,
      "additional_university_ids": [

      ],
      "discipline_id": 266,
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
      "updated_at": "2016-11-08T14:22:02.224Z",
      "shortname": "fu-course-202",
      "topic_id": 265,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 202",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 849,
      "id": 256,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 255,
      "additional_university_ids": [

      ],
      "discipline_id": 267,
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
      "updated_at": "2016-11-08T14:22:02.264Z",
      "shortname": "fu-course-203",
      "topic_id": 266,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bb1ce90b332e548dc1ce629ba8a3d2b31636ca983790ee49d4966ad14213cbb"
```
