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
DELETE /v2/chapters/81
Content-Type: application/json
Authorization: Bearer 81e2ce89f38d210561ae6d491cddab2110dc630d3e5e3452b505780264bcb5c5
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/81" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81e2ce89f38d210561ae6d491cddab2110dc630d3e5e3452b505780264bcb5c5"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/76
Content-Type: application/json
Authorization: Bearer ef3a8808592c27628bd423eb1226a61a6f102c6f449346e1b6300619c0586066
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
    "id": 76,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-08T12:16:22.147Z",
    "course_id": 132,
    "author_id": 359,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2015-03-12T14:00:00.000Z",
    "questions_updated_at": "2015-04-12T14:00:00.000Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 362,
        "chapter_id": 76,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T14:00:00.000Z",
        "created_at": "2016-09-08T12:16:22.111Z",
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
        "author_id": 363,
        "chapter_id": 76,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-09-08T12:16:22.142Z",
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
        "author_id": 360,
        "chapter_id": 76,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T14:00:00.000Z",
        "created_at": "2016-09-08T12:16:21.956Z",
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
        "author_id": 361,
        "chapter_id": 76,
        "position": 57,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-09-08T12:16:22.039Z",
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
curl "api.goskive.com/v2/chapters/76" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef3a8808592c27628bd423eb1226a61a6f102c6f449346e1b6300619c0586066"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/79
Content-Type: application/json
Authorization: Bearer c07ac5095582bbbf7d410990e3ff1238dbdd3c33049b10be54ad7737564bf0a6
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
    "id": 79,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-08T12:16:22.925Z",
    "course_id": 135,
    "author_id": 375,
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
curl "api.goskive.com/v2/chapters/79" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c07ac5095582bbbf7d410990e3ff1238dbdd3c33049b10be54ad7737564bf0a6"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer f6b8d6c70cee670db4d3a2b4177218082e54db956f6ff008a50b2c0841627e2b
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6b8d6c70cee670db4d3a2b4177218082e54db956f6ff008a50b2c0841627e2b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 0caf80b78d4cb65aa92ca313b500d4391ae9b3a374c2d982f2481bebb9893592
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
      "id": 22,
      "author_id": 633,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:43.264Z",
      "status": "published",
      "subject_id": 203,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 635,
      "reply_to_id": 22,
      "created_at": "2016-09-08T12:16:43.366Z",
      "status": "published",
      "subject_id": 204,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 637,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:43.463Z",
      "status": "published",
      "subject_id": 205,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 639,
      "reply_to_id": 24,
      "created_at": "2016-09-08T12:16:43.557Z",
      "status": "published",
      "subject_id": 206,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 641,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:43.652Z",
      "status": "reported",
      "subject_id": 207,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 643,
      "reply_to_id": 26,
      "created_at": "2016-09-08T12:16:43.743Z",
      "status": "published",
      "subject_id": 208,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 645,
      "reply_to_id": 26,
      "created_at": "2016-09-08T12:16:43.833Z",
      "status": "published",
      "subject_id": 209,
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
	-H "Authorization: Bearer 0caf80b78d4cb65aa92ca313b500d4391ae9b3a374c2d982f2481bebb9893592"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer fc42ef4651fdf569eb4f004b88c47870915958d16ad1f1a56971776b7eb51eb8
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
      "id": 29,
      "author_id": 648,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:44.009Z",
      "status": "published",
      "subject_id": 210,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 650,
      "reply_to_id": 29,
      "created_at": "2016-09-08T12:16:44.096Z",
      "status": "published",
      "subject_id": 211,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 652,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:44.186Z",
      "status": "published",
      "subject_id": 212,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 654,
      "reply_to_id": 31,
      "created_at": "2016-09-08T12:16:44.273Z",
      "status": "published",
      "subject_id": 213,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 656,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:44.361Z",
      "status": "reported",
      "subject_id": 214,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 658,
      "reply_to_id": 33,
      "created_at": "2016-09-08T12:16:44.447Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 660,
      "reply_to_id": 33,
      "created_at": "2016-09-08T12:16:44.535Z",
      "status": "published",
      "subject_id": 216,
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
	-H "Authorization: Bearer fc42ef4651fdf569eb4f004b88c47870915958d16ad1f1a56971776b7eb51eb8"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer cf29cda601df9a5ca24a28cb854e598203ad4b7b98f4dfe434b68fd91d88b75a
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
      "id": 16,
      "author_id": 620,
      "reply_to_id": 15,
      "created_at": "2016-09-08T12:16:42.611Z",
      "status": "published",
      "subject_id": 197,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 624,
      "reply_to_id": 17,
      "created_at": "2016-09-08T12:16:42.800Z",
      "status": "published",
      "subject_id": 199,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 628,
      "reply_to_id": 19,
      "created_at": "2016-09-08T12:16:42.985Z",
      "status": "published",
      "subject_id": 201,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 630,
      "reply_to_id": 19,
      "created_at": "2016-09-08T12:16:43.087Z",
      "status": "published",
      "subject_id": 202,
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
	-H "Authorization: Bearer cf29cda601df9a5ca24a28cb854e598203ad4b7b98f4dfe434b68fd91d88b75a"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer e53f26cc983750202bdf9d538ad55859bc5fe767bbbe7ad0edd1b1834ed8d3e4
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
      "id": 40,
      "author_id": 671,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:45.057Z",
      "status": "reported",
      "subject_id": 221,
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
	-H "Authorization: Bearer e53f26cc983750202bdf9d538ad55859bc5fe767bbbe7ad0edd1b1834ed8d3e4"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/50/republish
Content-Type: application/json
Authorization: Bearer cdbe96765f563348e74ce6ba31dee4a0ef934f8ee8118071268ca01817e05b51
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/50/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdbe96765f563348e74ce6ba31dee4a0ef934f8ee8118071268ca01817e05b51"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/251/chapters
Content-Type: application/json
Authorization: Bearer 894bbedbfd73c0cf717c99cbc29e92ff6a68d708f6c5dc52038ce5f183b7dd84
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
    "id": 139,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-08T12:16:49.513Z",
    "course_id": 251,
    "author_id": 758,
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
curl "api.goskive.com/v2/courses/251/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 894bbedbfd73c0cf717c99cbc29e92ff6a68d708f6c5dc52038ce5f183b7dd84"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5acb3316d6c7914c4bebeb562807ea6cfb3981d8b6213901f6e390e7b42b989b
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
    "id": 140,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-08T12:16:49.663Z",
    "course_id": 252,
    "author_id": 760,
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
	-H "Authorization: Bearer 5acb3316d6c7914c4bebeb562807ea6cfb3981d8b6213901f6e390e7b42b989b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 51db45afa7a11a07ca44e946a1a9ad4c757e3d586ffc378eb041c68e3f4b96b4
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
      "id": 157,
      "title": "Clever Chapter Title 136",
      "position": 1,
      "updated_at": "2016-09-08T12:16:51.607Z",
      "course_id": 263,
      "author_id": 798,
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
      "title": "Clever Chapter Title 137",
      "position": 2,
      "updated_at": "2016-09-08T12:16:51.631Z",
      "course_id": 263,
      "author_id": 799,
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
      "id": 159,
      "title": "Clever Chapter Title 138",
      "position": 3,
      "updated_at": "2016-09-08T12:16:51.753Z",
      "course_id": 263,
      "author_id": 800,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-09-08T12:16:51.683Z",
      "questions_updated_at": "2016-09-08T12:16:51.743Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51db45afa7a11a07ca44e946a1a9ad4c757e3d586ffc378eb041c68e3f4b96b4"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 58cd14a98e1c32401bbdf90603ed36249362a1bc6f375a70f936e3fe60ac645f
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
      "id": 160,
      "title": "Clever Chapter Title 139",
      "position": 1,
      "updated_at": "2016-09-08T12:16:52.034Z",
      "course_id": 265,
      "author_id": 807,
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
      "id": 161,
      "title": "Clever Chapter Title 140",
      "position": 2,
      "updated_at": "2016-09-08T12:16:52.058Z",
      "course_id": 265,
      "author_id": 808,
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
      "id": 162,
      "title": "Clever Chapter Title 141",
      "position": 3,
      "updated_at": "2016-09-08T12:16:52.082Z",
      "course_id": 265,
      "author_id": 809,
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
	-H "Authorization: Bearer 58cd14a98e1c32401bbdf90603ed36249362a1bc6f375a70f936e3fe60ac645f"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c2ab6b7b51dc5dc3e2bb5eb00f364b1d65d9bcbc468b904895e488c3a5966779
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
	-H "Authorization: Bearer c2ab6b7b51dc5dc3e2bb5eb00f364b1d65d9bcbc468b904895e488c3a5966779"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/85
Content-Type: application/json
Authorization: Bearer 5e2c2529673df31c6d92c5b235a21da5a606ae14edb20ce517188b701e068ebd
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/85" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e2c2529673df31c6d92c5b235a21da5a606ae14edb20ce517188b701e068ebd"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b45150ee565bfc6ba534712b65a9210886a72b1d4ab37c71b3bb256ad9c4b629
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
    "creator_id": 261,
    "id": 73,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 78,
    "additional_university_ids": [

    ],
    "topic_id": 80,
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
    "chapters_updated_at": "2016-09-08T12:16:13.876Z",
    "updated_at": "2016-09-08T12:16:13.878Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 59,
        "title": "Clever Chapter Title 59",
        "position": 1,
        "updated_at": "2016-09-08T12:16:13.847Z",
        "course_id": 73,
        "author_id": 261,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-08T12:16:13.843Z",
        "questions_updated_at": "2016-09-08T12:16:13.661Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 60,
        "title": "Clever Chapter Title 60",
        "position": 2,
        "updated_at": "2016-09-08T12:16:13.876Z",
        "course_id": 73,
        "author_id": 261,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-08T12:16:13.872Z",
        "questions_updated_at": "2016-09-08T12:16:13.722Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 261,
        "chapter_id": 59,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.747Z",
        "created_at": "2016-09-08T12:16:13.747Z",
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
        "author_id": 261,
        "chapter_id": 60,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.790Z",
        "created_at": "2016-09-08T12:16:13.790Z",
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
        "author_id": 261,
        "chapter_id": 59,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.769Z",
        "created_at": "2016-09-08T12:16:13.769Z",
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
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 261,
        "chapter_id": 60,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.814Z",
        "created_at": "2016-09-08T12:16:13.814Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 264,
        "chapter_id": 59,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.843Z",
        "created_at": "2016-09-08T12:16:13.843Z",
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
        "author_id": 265,
        "chapter_id": 60,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:13.872Z",
        "created_at": "2016-09-08T12:16:13.872Z",
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
	-H "Authorization: Bearer b45150ee565bfc6ba534712b65a9210886a72b1d4ab37c71b3bb256ad9c4b629"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/67
Content-Type: application/json
Authorization: Bearer f7c79e9601827bf379fdcc98f9b9b6758d2022232346f405874d929e3ada295d
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
    "creator_id": 247,
    "id": 67,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 72,
    "additional_university_ids": [

    ],
    "topic_id": 74,
    "discipline_id": 75,
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
    "updated_at": "2016-09-08T12:16:11.995Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/67" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7c79e9601827bf379fdcc98f9b9b6758d2022232346f405874d929e3ada295d"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7efdbd37b585c5d9d4e9fbd17c060e7812a84d4edb3e54572daf74b57b342c57
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
    "creator_id": 252,
    "id": 70,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 75,
    "additional_university_ids": [

    ],
    "topic_id": 77,
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
    "updated_at": "2016-09-08T12:16:12.449Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7efdbd37b585c5d9d4e9fbd17c060e7812a84d4edb3e54572daf74b57b342c57"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer d1223edf97d08f89607926617dff7148c7f8c03f8577c9fffbb77a207c4fd2db
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
      "id": 29,
      "user_id": 528,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:31.140Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 532,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:31.337Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 536,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:31.510Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 540,
      "feedbackable_id": 84,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:31.683Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 544,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-08T12:16:31.852Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1223edf97d08f89607926617dff7148c7f8c03f8577c9fffbb77a207c4fd2db"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer be0c12a2303de7e6c27a39c6bb6a20bc561f33e84032217f559a63a38dcf4570
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
      "id": 38,
      "user_id": 565,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-08T12:16:32.829Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be0c12a2303de7e6c27a39c6bb6a20bc561f33e84032217f559a63a38dcf4570"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/83/feedbacks
Content-Type: application/json
Authorization: Bearer d485b1b16937c351215b72a04328929a588a174912b95ca978296899dc9be71b
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
      "user_id": 750,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:48.749Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 749,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:48.733Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d485b1b16937c351215b72a04328929a588a174912b95ca978296899dc9be71b"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 7aaa9c1117b6344b9602e19a342fec709b18136a4433e2a9293a892b1b9ec544
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
      "updated_at": "2016-09-08T12:15:55.834Z",
      "created_at": "2016-09-08T12:15:55.834Z",
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
      "updated_at": "2016-09-08T12:15:55.949Z",
      "created_at": "2016-09-08T12:15:55.949Z",
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
      "updated_at": "2016-09-08T12:15:56.064Z",
      "created_at": "2016-09-08T12:15:56.064Z",
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
      "updated_at": "2016-09-08T12:15:56.177Z",
      "created_at": "2016-09-08T12:15:56.177Z",
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
      "updated_at": "2016-09-08T12:15:56.308Z",
      "created_at": "2016-09-08T12:15:56.308Z",
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
	-H "Authorization: Bearer 7aaa9c1117b6344b9602e19a342fec709b18136a4433e2a9293a892b1b9ec544"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer ca715531dfd76df13b8d4b1322f1a75f8c9492802dab52441fae85eb32d73a35
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
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 32,
      "chapter_id": 10,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:15:55.669Z",
      "created_at": "2016-09-08T12:15:55.669Z",
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
	-H "Authorization: Bearer ca715531dfd76df13b8d4b1322f1a75f8c9492802dab52441fae85eb32d73a35"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/17/republish
Content-Type: application/json
Authorization: Bearer 680a556f6fc136fe3cbc11c73ec053ac6e62ddf32ef0323449937910dbeb8308
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/17/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 680a556f6fc136fe3cbc11c73ec053ac6e62ddf32ef0323449937910dbeb8308"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/11/feedbacks
Content-Type: application/json
Authorization: Bearer 47c10c0493bed47629adc878d43b9baeea52e575160455a4f05f7611bc727883
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
      "user_id": 148,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:04.312Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 147,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:04.299Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/11/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47c10c0493bed47629adc878d43b9baeea52e575160455a4f05f7611bc727883"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer f5419419b2e9ce73bba0fe389ce1741e6434e2621cee397028b2967051f57005
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
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 868,
      "chapter_id": 178,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.808Z",
      "created_at": "2016-09-08T12:16:55.783Z",
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
          "id": 233,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 234,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 859,
      "chapter_id": 175,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.337Z",
      "created_at": "2016-09-08T12:16:55.311Z",
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
          "id": 227,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 228,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 862,
      "chapter_id": 176,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.500Z",
      "created_at": "2016-09-08T12:16:55.474Z",
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
          "id": 229,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 230,
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
      "author_id": 865,
      "chapter_id": 177,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.656Z",
      "created_at": "2016-09-08T12:16:55.630Z",
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
          "id": 231,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 232,
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
      "author_id": 871,
      "chapter_id": 179,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.962Z",
      "created_at": "2016-09-08T12:16:55.938Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5419419b2e9ce73bba0fe389ce1741e6434e2621cee397028b2967051f57005"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 5f97a92b52f57935aad1e8e4db60094cd5394d3248bb357fbef1b4c14ad8ceb0
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
      "id": 111,
      "obfuscated_id": "G-D-sgMUtTw",
      "author_id": 855,
      "chapter_id": 174,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:55.099Z",
      "created_at": "2016-09-08T12:16:55.072Z",
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
          "id": 225,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 226,
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
	-H "Authorization: Bearer 5f97a92b52f57935aad1e8e4db60094cd5394d3248bb357fbef1b4c14ad8ceb0"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/103/republish
Content-Type: application/json
Authorization: Bearer 1100aae3b6ae19241b117b373ac9297479c935c2a3f252d3dfd8b128adda4ef1
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/103/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1100aae3b6ae19241b117b373ac9297479c935c2a3f252d3dfd8b128adda4ef1"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2ede189752449880adb085a3952656deac0d692614067afba5955d8674227221
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":135,"published":false}}
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
    "creator_id": 352,
    "id": 128,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 112,
    "additional_university_ids": [

    ],
    "topic_id": 135,
    "discipline_id": 136,
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
    "updated_at": "2016-09-08T12:16:21.372Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":135,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ede189752449880adb085a3952656deac0d692614067afba5955d8674227221"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cdf0398f4b20941f7c412a38e4823986b4fc2e8701a5723c3d3ac2790a26d418
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
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-67",
      "html_url": "https://goskive.com/course/fu-course-67",
      "slug": "fu-course-67",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "topic_id": 97,
      "discipline_id": 98,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
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
      "updated_at": "2016-09-08T12:16:17.638Z",
      "shortname": "fu-course-67"
    },
    {
      "creator_id": 309,
      "id": 91,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-68",
      "html_url": "https://goskive.com/course/fu-course-68",
      "slug": "fu-course-68",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "topic_id": 98,
      "discipline_id": 99,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
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
      "updated_at": "2016-09-08T12:16:17.678Z",
      "shortname": "fu-course-68"
    },
    {
      "creator_id": 310,
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-69",
      "html_url": "https://goskive.com/course/fu-course-69",
      "slug": "fu-course-69",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "topic_id": 99,
      "discipline_id": 100,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 69",
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
      "updated_at": "2016-09-08T12:16:17.729Z",
      "shortname": "fu-course-69"
    },
    {
      "creator_id": 310,
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-70",
      "html_url": "https://goskive.com/course/fu-course-70",
      "slug": "fu-course-70",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "topic_id": 100,
      "discipline_id": 101,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 70",
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
      "chapters_updated_at": "2016-09-08T12:16:17.890Z",
      "updated_at": "2016-09-08T12:16:17.892Z",
      "shortname": "fu-course-70"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdf0398f4b20941f7c412a38e4823986b4fc2e8701a5723c3d3ac2790a26d418"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f1ce11820b285f2badac882269e3b897e6e8f1e2b527061c3fcdd1631f0becf8
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
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-71",
      "html_url": "https://goskive.com/course/fu-course-71",
      "slug": "fu-course-71",
      "university_id": 98,
      "additional_university_ids": [

      ],
      "topic_id": 101,
      "discipline_id": 102,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 71",
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
      "updated_at": "2016-09-08T12:16:18.117Z",
      "shortname": "fu-course-71"
    },
    {
      "creator_id": 316,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-72",
      "html_url": "https://goskive.com/course/fu-course-72",
      "slug": "fu-course-72",
      "university_id": 98,
      "additional_university_ids": [

      ],
      "topic_id": 102,
      "discipline_id": 103,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 72",
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
      "updated_at": "2016-09-08T12:16:18.161Z",
      "shortname": "fu-course-72"
    },
    {
      "creator_id": 317,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-73",
      "html_url": "https://goskive.com/course/fu-course-73",
      "slug": "fu-course-73",
      "university_id": 98,
      "additional_university_ids": [

      ],
      "topic_id": 103,
      "discipline_id": 104,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 73",
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
      "updated_at": "2016-09-08T12:16:18.214Z",
      "shortname": "fu-course-73"
    },
    {
      "creator_id": 317,
      "id": 97,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-74",
      "html_url": "https://goskive.com/course/fu-course-74",
      "slug": "fu-course-74",
      "university_id": 98,
      "additional_university_ids": [

      ],
      "topic_id": 104,
      "discipline_id": 105,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 74",
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
      "updated_at": "2016-09-08T12:16:18.256Z",
      "shortname": "fu-course-74"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1ce11820b285f2badac882269e3b897e6e8f1e2b527061c3fcdd1631f0becf8"
```
