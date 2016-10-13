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
DELETE /v2/chapters/193
Content-Type: application/json
Authorization: Bearer a3ffb917168793451f9bdd2b65bcecabe95eea7d1d8b9446e8c15e60f7ca0bfe
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/193" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3ffb917168793451f9bdd2b65bcecabe95eea7d1d8b9446e8c15e60f7ca0bfe"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 59f245a45044a0d4af7707ff68ac9535b4051588294926f1b5d4e975ad26e521
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
    "id": 191,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T18:22:25.986Z",
    "course_id": 297,
    "author_id": 935,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-13T18:22:25.399Z",
    "questions_updated_at": "2016-10-13T18:22:25.399Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 94,
        "obfuscated_id": "CVi6VU_nV6k",
        "author_id": 938,
        "chapter_id": 191,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.926Z",
        "created_at": "2016-10-13T18:22:25.926Z",
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
        "author_id": 939,
        "chapter_id": 191,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.967Z",
        "created_at": "2016-10-13T18:22:25.967Z",
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
        "id": 131,
        "obfuscated_id": "gCw8isdgMKE",
        "author_id": 936,
        "chapter_id": 191,
        "position": 118,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.638Z",
        "created_at": "2016-10-13T18:22:25.522Z",
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
            "id": 265,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 266,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 132,
        "obfuscated_id": "RECRPLqMrqE",
        "author_id": 937,
        "chapter_id": 191,
        "position": 119,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.850Z",
        "created_at": "2016-10-13T18:22:25.717Z",
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
            "id": 267,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 268,
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
curl "api.goskive.com/v2/chapters/191" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59f245a45044a0d4af7707ff68ac9535b4051588294926f1b5d4e975ad26e521"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/187
Content-Type: application/json
Authorization: Bearer f8bff289650ccb77dec10994da0572ef3af32b01e40eae433fa28935ccf25808
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
    "id": 187,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T18:22:24.336Z",
    "course_id": 293,
    "author_id": 920,
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
curl "api.goskive.com/v2/chapters/187" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8bff289650ccb77dec10994da0572ef3af32b01e40eae433fa28935ccf25808"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 2cf66ee2b5ee31f08a7f00b124303af4b7ed21df1c448eefa03d6e617a83d202
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cf66ee2b5ee31f08a7f00b124303af4b7ed21df1c448eefa03d6e617a83d202"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5388415c747f81ae3a532ede3d3b836113011d1fefdcf81a1275bbe48af32de2
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
      "id": 12,
      "author_id": 218,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:21.447Z",
      "status": "published",
      "subject_id": 56,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 220,
      "reply_to_id": 12,
      "created_at": "2016-10-13T18:21:21.538Z",
      "status": "published",
      "subject_id": 57,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 222,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:21.630Z",
      "status": "published",
      "subject_id": 58,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 224,
      "reply_to_id": 14,
      "created_at": "2016-10-13T18:21:21.718Z",
      "status": "published",
      "subject_id": 59,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 226,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:21.805Z",
      "status": "reported",
      "subject_id": 60,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 228,
      "reply_to_id": 16,
      "created_at": "2016-10-13T18:21:21.893Z",
      "status": "published",
      "subject_id": 61,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 230,
      "reply_to_id": 16,
      "created_at": "2016-10-13T18:21:21.981Z",
      "status": "published",
      "subject_id": 62,
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
	-H "Authorization: Bearer 5388415c747f81ae3a532ede3d3b836113011d1fefdcf81a1275bbe48af32de2"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 47c21f1a6795e855839748a60ce5e047a35646f38343ce9561bda2946a6bbbe0
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
      "author_id": 278,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:24.193Z",
      "status": "published",
      "subject_id": 84,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 280,
      "reply_to_id": 40,
      "created_at": "2016-10-13T18:21:24.283Z",
      "status": "published",
      "subject_id": 85,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 282,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:24.375Z",
      "status": "published",
      "subject_id": 86,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 284,
      "reply_to_id": 42,
      "created_at": "2016-10-13T18:21:24.466Z",
      "status": "published",
      "subject_id": 87,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 286,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:24.557Z",
      "status": "reported",
      "subject_id": 88,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 288,
      "reply_to_id": 44,
      "created_at": "2016-10-13T18:21:24.649Z",
      "status": "published",
      "subject_id": 89,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 290,
      "reply_to_id": 44,
      "created_at": "2016-10-13T18:21:24.741Z",
      "status": "published",
      "subject_id": 90,
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
	-H "Authorization: Bearer 47c21f1a6795e855839748a60ce5e047a35646f38343ce9561bda2946a6bbbe0"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e5b6fc0fe5cfda61d12e6a0fe5bd1e60c6d30e2daa0cb46daf51a7e6e0bd089c
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
      "author_id": 235,
      "reply_to_id": 19,
      "created_at": "2016-10-13T18:21:22.219Z",
      "status": "published",
      "subject_id": 64,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 239,
      "reply_to_id": 21,
      "created_at": "2016-10-13T18:21:22.396Z",
      "status": "published",
      "subject_id": 66,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 243,
      "reply_to_id": 23,
      "created_at": "2016-10-13T18:21:22.575Z",
      "status": "published",
      "subject_id": 68,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 245,
      "reply_to_id": 23,
      "created_at": "2016-10-13T18:21:22.666Z",
      "status": "published",
      "subject_id": 69,
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
	-H "Authorization: Bearer e5b6fc0fe5cfda61d12e6a0fe5bd1e60c6d30e2daa0cb46daf51a7e6e0bd089c"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 92bb86105b2335485caaf72158a772d178b78137b29dc6602f52bfcfd7c457bf
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
      "id": 37,
      "author_id": 271,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:23.876Z",
      "status": "reported",
      "subject_id": 81,
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
	-H "Authorization: Bearer 92bb86105b2335485caaf72158a772d178b78137b29dc6602f52bfcfd7c457bf"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/11/republish
Content-Type: application/json
Authorization: Bearer 45a1b63de67c828998e479b8af4d473dfa32fde8ccd06dc7a9338ee26da0d903
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
	-H "Authorization: Bearer 45a1b63de67c828998e479b8af4d473dfa32fde8ccd06dc7a9338ee26da0d903"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 36332b4ffe9b61ba62efab39b1da44bb9310ddabaf0d224a243ddaebf56c7b08
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
    "id": 132,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T18:22:00.541Z",
    "course_id": 228,
    "author_id": 690,
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
	-H "Authorization: Bearer 36332b4ffe9b61ba62efab39b1da44bb9310ddabaf0d224a243ddaebf56c7b08"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/229/chapters
Content-Type: application/json
Authorization: Bearer 6f1a00adb586865e7773c42780d6762cf85f089ba122fa789afcee92dd734e08
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
    "id": 133,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T18:22:00.687Z",
    "course_id": 229,
    "author_id": 692,
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
curl "api.goskive.com/v2/courses/229/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f1a00adb586865e7773c42780d6762cf85f089ba122fa789afcee92dd734e08"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4cec5d92a4d678cfe20bf7900e88a479090f19585993ca1fbadf22f02f73f9cc
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
      "id": 113,
      "title": "Clever Chapter Title 101",
      "position": 1,
      "updated_at": "2016-10-13T18:21:57.912Z",
      "course_id": 217,
      "author_id": 647,
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
      "id": 114,
      "title": "Clever Chapter Title 102",
      "position": 2,
      "updated_at": "2016-10-13T18:21:57.939Z",
      "course_id": 217,
      "author_id": 648,
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
      "id": 115,
      "title": "Clever Chapter Title 103",
      "position": 3,
      "updated_at": "2016-10-13T18:21:58.217Z",
      "course_id": 217,
      "author_id": 649,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-13T18:21:57.828Z",
      "questions_updated_at": "2016-10-13T18:21:57.828Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cec5d92a4d678cfe20bf7900e88a479090f19585993ca1fbadf22f02f73f9cc"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2ec976b72181c6990b33b23d41ccd60a8cbe076a27a4bba26baeb7fb8cefb4c6
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
      "id": 116,
      "title": "Clever Chapter Title 104",
      "position": 1,
      "updated_at": "2016-10-13T18:21:58.496Z",
      "course_id": 219,
      "author_id": 656,
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
      "id": 117,
      "title": "Clever Chapter Title 105",
      "position": 2,
      "updated_at": "2016-10-13T18:21:58.524Z",
      "course_id": 219,
      "author_id": 657,
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
      "id": 118,
      "title": "Clever Chapter Title 106",
      "position": 3,
      "updated_at": "2016-10-13T18:21:58.551Z",
      "course_id": 219,
      "author_id": 658,
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
	-H "Authorization: Bearer 2ec976b72181c6990b33b23d41ccd60a8cbe076a27a4bba26baeb7fb8cefb4c6"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 249ab760b8128f019b736b13edc6b0df294d897a2476b11fdb5e232581b53c06
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
	-H "Authorization: Bearer 249ab760b8128f019b736b13edc6b0df294d897a2476b11fdb5e232581b53c06"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/287
Content-Type: application/json
Authorization: Bearer 14dcb3028183f7cccd5ebff4faaa563f0f9c2f1b12afc63baa66558e4c4c04fa
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/287" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14dcb3028183f7cccd5ebff4faaa563f0f9c2f1b12afc63baa66558e4c4c04fa"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 114ec5f51ebbdd868c31d4679930750bdc1739234b8adf22116b6fd0a8711fe6
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
    "id": 291,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 276,
    "additional_university_ids": [

    ],
    "topic_id": 303,
    "discipline_id": 304,
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
    "chapters_updated_at": "2016-10-13T18:22:20.844Z",
    "updated_at": "2016-10-13T18:22:22.370Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 183,
        "title": "Clever Chapter Title 168",
        "position": 1,
        "updated_at": "2016-10-13T18:22:22.317Z",
        "course_id": 291,
        "author_id": 907,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T18:22:20.844Z",
        "questions_updated_at": "2016-10-13T18:22:20.844Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 184,
        "title": "Clever Chapter Title 169",
        "position": 2,
        "updated_at": "2016-10-13T18:22:22.362Z",
        "course_id": 291,
        "author_id": 907,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T18:22:20.844Z",
        "questions_updated_at": "2016-10-13T18:22:20.844Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 907,
        "chapter_id": 183,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.140Z",
        "created_at": "2016-10-13T18:22:22.140Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 907,
        "chapter_id": 184,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.218Z",
        "created_at": "2016-10-13T18:22:22.218Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 907,
        "chapter_id": 183,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.184Z",
        "created_at": "2016-10-13T18:22:22.184Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 907,
        "chapter_id": 184,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.262Z",
        "created_at": "2016-10-13T18:22:22.262Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 910,
        "chapter_id": 183,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.307Z",
        "created_at": "2016-10-13T18:22:22.307Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 911,
        "chapter_id": 184,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.351Z",
        "created_at": "2016-10-13T18:22:22.351Z",
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
	-H "Authorization: Bearer 114ec5f51ebbdd868c31d4679930750bdc1739234b8adf22116b6fd0a8711fe6"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/274
Content-Type: application/json
Authorization: Bearer dc3cd0df5d061c04af20f75f33381e8418a7b1ff8a9dee04bb696b79c30d8c7f
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
    "creator_id": 865,
    "id": 274,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 259,
    "additional_university_ids": [

    ],
    "topic_id": 286,
    "discipline_id": 287,
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
    "updated_at": "2016-10-13T18:22:15.219Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/274" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc3cd0df5d061c04af20f75f33381e8418a7b1ff8a9dee04bb696b79c30d8c7f"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a1f500523a5f00be0ff21d841ddc54efe2854ed8083f13e688abe9ae010f0f60
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
    "creator_id": 867,
    "id": 275,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 260,
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
    "updated_at": "2016-10-13T18:22:15.373Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1f500523a5f00be0ff21d841ddc54efe2854ed8083f13e688abe9ae010f0f60"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 164bec4d9d740c953c73dd5e42539057af54c1696ed596036749be55ec154c72
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
      "user_id": 113,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:14.675Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 117,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:14.997Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 121,
      "feedbackable_id": 20,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:15.325Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 125,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:15.654Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 129,
      "feedbackable_id": 22,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T18:21:15.989Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 164bec4d9d740c953c73dd5e42539057af54c1696ed596036749be55ec154c72"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 9c7f5761568e4dafa1d22f0d73cdc09613d6699a3e3ba573a283b4f46fecbf9d
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
      "id": 20,
      "user_id": 150,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T18:21:17.696Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c7f5761568e4dafa1d22f0d73cdc09613d6699a3e3ba573a283b4f46fecbf9d"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/3
Authorization: Bearer 7fa2b1bf23345eda797d62e3d3de18b3bddcd0659e13d5b5be62363c7bd88dfe
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
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Authorization: Bearer 7fa2b1bf23345eda797d62e3d3de18b3bddcd0659e13d5b5be62363c7bd88dfe" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/28/feedbacks
Content-Type: application/json
Authorization: Bearer d7d56b1b2f1d87cdea68f9fe1d5784ef600dc61e21618e657e831a6fddf988c1
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
      "user_id": 561,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:50.614Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 560,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:50.600Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/28/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7d56b1b2f1d87cdea68f9fe1d5784ef600dc61e21618e657e831a6fddf988c1"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 64c672194684db71368067d68cd2f1e5c801288418fa157c744eea338c1df9f7
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 776,
      "chapter_id": 154,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:06.959Z",
      "created_at": "2016-10-13T18:22:06.959Z",
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
      "author_id": 779,
      "chapter_id": 155,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:07.112Z",
      "created_at": "2016-10-13T18:22:07.112Z",
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
      "author_id": 782,
      "chapter_id": 156,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:07.270Z",
      "created_at": "2016-10-13T18:22:07.270Z",
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
      "author_id": 785,
      "chapter_id": 157,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:07.424Z",
      "created_at": "2016-10-13T18:22:07.424Z",
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
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 788,
      "chapter_id": 158,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:07.571Z",
      "created_at": "2016-10-13T18:22:07.571Z",
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
	-H "Authorization: Bearer 64c672194684db71368067d68cd2f1e5c801288418fa157c744eea338c1df9f7"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer af449aadf6249d21f677c0c62cd381e2baad140538b9d7336e27d0f67649df6d
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 772,
      "chapter_id": 153,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:22:06.764Z",
      "created_at": "2016-10-13T18:22:06.764Z",
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
	-H "Authorization: Bearer af449aadf6249d21f677c0c62cd381e2baad140538b9d7336e27d0f67649df6d"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/62/republish
Content-Type: application/json
Authorization: Bearer 399c7ab04f487411fe0d8e2f19674034c4d40a4719f59da7ccaf2f45ccbb4170
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/62/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 399c7ab04f487411fe0d8e2f19674034c4d40a4719f59da7ccaf2f45ccbb4170"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/100/feedbacks
Content-Type: application/json
Authorization: Bearer 9891046e4c30f8b6dd96d709002bd19839fe98ca436cc35835cbaac784f5b7a9
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
      "user_id": 858,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:22:14.054Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 857,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:22:14.040Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/100/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9891046e4c30f8b6dd96d709002bd19839fe98ca436cc35835cbaac784f5b7a9"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 4b9f9801f50cbffe4115f4abc5eae7c57fb2dc1be2cf48815728dca9fb3cec5b
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 482,
      "chapter_id": 68,
      "position": 46,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:42.263Z",
      "created_at": "2016-10-13T18:21:42.141Z",
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
          "id": 101,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 102,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 476,
      "chapter_id": 66,
      "position": 44,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:41.662Z",
      "created_at": "2016-10-13T18:21:41.539Z",
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
          "id": 97,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 98,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 479,
      "chapter_id": 67,
      "position": 45,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:41.963Z",
      "created_at": "2016-10-13T18:21:41.841Z",
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
          "id": 99,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 100,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 485,
      "chapter_id": 69,
      "position": 47,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:42.564Z",
      "created_at": "2016-10-13T18:21:42.442Z",
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
          "id": 103,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 104,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 488,
      "chapter_id": 70,
      "position": 48,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:42.855Z",
      "created_at": "2016-10-13T18:21:42.741Z",
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
          "id": 105,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 106,
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
	-H "Authorization: Bearer 4b9f9801f50cbffe4115f4abc5eae7c57fb2dc1be2cf48815728dca9fb3cec5b"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 8105220448134fef0799c22f175b6ecaa9f0979f9a2a6373d408c22b9fa0f6b9
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 504,
      "chapter_id": 75,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:44.485Z",
      "created_at": "2016-10-13T18:21:44.369Z",
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
          "id": 115,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 116,
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
	-H "Authorization: Bearer 8105220448134fef0799c22f175b6ecaa9f0979f9a2a6373d408c22b9fa0f6b9"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/65/republish
Content-Type: application/json
Authorization: Bearer 316e2a3aa292e7b74de34e682333121c60abb98967490231900ee2ed1cbee0cd
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 316e2a3aa292e7b74de34e682333121c60abb98967490231900ee2ed1cbee0cd"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer beaf3b04d0b8b93a70a5d39e2c70e90c2d16b870f2759cb897e986852fe079e7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":124,"published":false}}
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
    "creator_id": 384,
    "id": 119,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 126,
    "additional_university_ids": [

    ],
    "topic_id": 124,
    "discipline_id": 124,
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
    "updated_at": "2016-10-13T18:21:33.055Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":124,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer beaf3b04d0b8b93a70a5d39e2c70e90c2d16b870f2759cb897e986852fe079e7"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3d596de8adc1e4d9dc03f17792541be72f2d93bc277b9a6e59372d3028e9577a
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
      "creator_id": 412,
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 149,
      "discipline_id": 149,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 120",
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
      "updated_at": "2016-10-13T18:21:35.880Z",
      "shortname": "fu-course-120"
    },
    {
      "creator_id": 412,
      "id": 145,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-121",
      "html_url": "https://goskive.com/course/fu-course-121",
      "slug": "fu-course-121",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 150,
      "discipline_id": 150,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 121",
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
      "updated_at": "2016-10-13T18:21:35.923Z",
      "shortname": "fu-course-121"
    },
    {
      "creator_id": 413,
      "id": 146,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 151,
      "discipline_id": 151,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 122",
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
      "updated_at": "2016-10-13T18:21:35.975Z",
      "shortname": "fu-course-122"
    },
    {
      "creator_id": 413,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 152,
      "discipline_id": 152,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "chapters_updated_at": "2016-10-13T18:21:36.283Z",
      "updated_at": "2016-10-13T18:21:36.289Z",
      "shortname": "fu-course-123"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d596de8adc1e4d9dc03f17792541be72f2d93bc277b9a6e59372d3028e9577a"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 93cc5c87c1dc813fcc93b37790322157917b909c2395ecf69ac31fe4cc1f5112
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
      "creator_id": 418,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-124",
      "html_url": "https://goskive.com/course/fu-course-124",
      "slug": "fu-course-124",
      "university_id": 137,
      "additional_university_ids": [

      ],
      "topic_id": 153,
      "discipline_id": 153,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 124",
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
      "updated_at": "2016-10-13T18:21:36.448Z",
      "shortname": "fu-course-124"
    },
    {
      "creator_id": 418,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-125",
      "html_url": "https://goskive.com/course/fu-course-125",
      "slug": "fu-course-125",
      "university_id": 137,
      "additional_university_ids": [

      ],
      "topic_id": 154,
      "discipline_id": 154,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 125",
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
      "updated_at": "2016-10-13T18:21:36.494Z",
      "shortname": "fu-course-125"
    },
    {
      "creator_id": 419,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 137,
      "additional_university_ids": [

      ],
      "topic_id": 155,
      "discipline_id": 155,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "updated_at": "2016-10-13T18:21:36.548Z",
      "shortname": "fu-course-126"
    },
    {
      "creator_id": 419,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 137,
      "additional_university_ids": [

      ],
      "topic_id": 156,
      "discipline_id": 156,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-10-13T18:21:36.592Z",
      "shortname": "fu-course-127"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93cc5c87c1dc813fcc93b37790322157917b909c2395ecf69ac31fe4cc1f5112"
```
