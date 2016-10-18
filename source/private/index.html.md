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
DELETE /v2/chapters/54
Content-Type: application/json
Authorization: Bearer 069f0fe4dae25b6b380c6360a0dc49a50aa0ed19e739c7cfade2a413795528b5
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 069f0fe4dae25b6b380c6360a0dc49a50aa0ed19e739c7cfade2a413795528b5"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/59
Content-Type: application/json
Authorization: Bearer b4270b2d71bad182f3c47f9bccf79679987bc786bdbda5fe70b9b1a01fe21487
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
    "id": 59,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T16:43:39.968Z",
    "course_id": 119,
    "author_id": 335,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-18T16:43:39.376Z",
    "questions_updated_at": "2016-10-18T16:43:39.376Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 338,
        "chapter_id": 59,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:43:39.906Z",
        "created_at": "2016-10-18T16:43:39.906Z",
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
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 339,
        "chapter_id": 59,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:43:39.947Z",
        "created_at": "2016-10-18T16:43:39.947Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 336,
        "chapter_id": 59,
        "position": 29,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:43:39.611Z",
        "created_at": "2016-10-18T16:43:39.487Z",
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
            "id": 57,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 58,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 337,
        "chapter_id": 59,
        "position": 30,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:43:39.826Z",
        "created_at": "2016-10-18T16:43:39.691Z",
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
            "id": 59,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 60,
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
curl "api.goskive.com/v2/chapters/59" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4270b2d71bad182f3c47f9bccf79679987bc786bdbda5fe70b9b1a01fe21487"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/55
Content-Type: application/json
Authorization: Bearer b35ee2e78c9bd0bebb025b2be9a135043b9befeb4a7f908d9f8eda07691189a2
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
    "id": 55,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T16:43:38.378Z",
    "course_id": 115,
    "author_id": 320,
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
curl "api.goskive.com/v2/chapters/55" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b35ee2e78c9bd0bebb025b2be9a135043b9befeb4a7f908d9f8eda07691189a2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer cca8bef7754b4afda83bdd37575433a56fb66db8fb05f5b1c6f189acab589c81
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cca8bef7754b4afda83bdd37575433a56fb66db8fb05f5b1c6f189acab589c81"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e62ff77c1eeeb346ed38afd10d923b7432a381154ce33dde853fe5a52bb82d65
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
      "id": 14,
      "author_id": 645,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:10.901Z",
      "status": "published",
      "subject_id": 205,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 647,
      "reply_to_id": 14,
      "created_at": "2016-10-18T16:44:10.989Z",
      "status": "published",
      "subject_id": 206,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 649,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:11.079Z",
      "status": "published",
      "subject_id": 207,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 651,
      "reply_to_id": 16,
      "created_at": "2016-10-18T16:44:11.168Z",
      "status": "published",
      "subject_id": 208,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 653,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:11.259Z",
      "status": "reported",
      "subject_id": 209,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 655,
      "reply_to_id": 18,
      "created_at": "2016-10-18T16:44:11.344Z",
      "status": "published",
      "subject_id": 210,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 657,
      "reply_to_id": 18,
      "created_at": "2016-10-18T16:44:11.434Z",
      "status": "published",
      "subject_id": 211,
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
	-H "Authorization: Bearer e62ff77c1eeeb346ed38afd10d923b7432a381154ce33dde853fe5a52bb82d65"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 297bee82c4a549da95f4a5f6c66ce7c88d925080980544c7b0653d07736750fe
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
      "id": 42,
      "author_id": 705,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:13.559Z",
      "status": "published",
      "subject_id": 233,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 707,
      "reply_to_id": 42,
      "created_at": "2016-10-18T16:44:13.645Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 709,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:13.733Z",
      "status": "published",
      "subject_id": 235,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 711,
      "reply_to_id": 44,
      "created_at": "2016-10-18T16:44:13.817Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 713,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:13.904Z",
      "status": "reported",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 715,
      "reply_to_id": 46,
      "created_at": "2016-10-18T16:44:13.991Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 717,
      "reply_to_id": 46,
      "created_at": "2016-10-18T16:44:14.105Z",
      "status": "published",
      "subject_id": 239,
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
	-H "Authorization: Bearer 297bee82c4a549da95f4a5f6c66ce7c88d925080980544c7b0653d07736750fe"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 1b5df6d07f98f874f267f0e7d2a21b5270f96d69cbf93e573f2720bbaa27f47a
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
      "id": 22,
      "author_id": 662,
      "reply_to_id": 21,
      "created_at": "2016-10-18T16:44:11.666Z",
      "status": "published",
      "subject_id": 213,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 666,
      "reply_to_id": 23,
      "created_at": "2016-10-18T16:44:11.867Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 670,
      "reply_to_id": 25,
      "created_at": "2016-10-18T16:44:12.042Z",
      "status": "published",
      "subject_id": 217,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 672,
      "reply_to_id": 25,
      "created_at": "2016-10-18T16:44:12.131Z",
      "status": "published",
      "subject_id": 218,
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
	-H "Authorization: Bearer 1b5df6d07f98f874f267f0e7d2a21b5270f96d69cbf93e573f2720bbaa27f47a"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer f01feb8772da7f759c92ad7a8144ffaee522fcd74012ddeabfbf680b6d9b5497
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
      "id": 39,
      "author_id": 698,
      "reply_to_id": null,
      "created_at": "2016-10-18T16:44:13.262Z",
      "status": "reported",
      "subject_id": 230,
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
	-H "Authorization: Bearer f01feb8772da7f759c92ad7a8144ffaee522fcd74012ddeabfbf680b6d9b5497"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/49/republish
Content-Type: application/json
Authorization: Bearer 50898ad67bc927ee2621910ab1ef694cde6f7f20078e0dfe6f3726d2d142580d
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50898ad67bc927ee2621910ab1ef694cde6f7f20078e0dfe6f3726d2d142580d"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 68d12e569c3608545f97c756d916880479d0e5c3e5f0dd60144dc608b061bdce
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
    "id": 131,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T16:44:16.148Z",
    "course_id": 250,
    "author_id": 751,
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
	-H "Authorization: Bearer 68d12e569c3608545f97c756d916880479d0e5c3e5f0dd60144dc608b061bdce"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/251/chapters
Content-Type: application/json
Authorization: Bearer b501a796ecd581dd87717c45438e8927b74099dbaa3afe8edecf02d473ad0b75
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
    "updated_at": "2016-10-18T16:44:16.290Z",
    "course_id": 251,
    "author_id": 753,
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
	-H "Authorization: Bearer b501a796ecd581dd87717c45438e8927b74099dbaa3afe8edecf02d473ad0b75"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 330d9d5729cdc7abe1cac1aa5d15db1a8c1832f8888a071fc684484e2ae39433
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
      "id": 133,
      "title": "Clever Chapter Title 109",
      "position": 1,
      "updated_at": "2016-10-18T16:44:16.404Z",
      "course_id": 252,
      "author_id": 755,
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
      "id": 134,
      "title": "Clever Chapter Title 110",
      "position": 2,
      "updated_at": "2016-10-18T16:44:16.429Z",
      "course_id": 252,
      "author_id": 756,
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
      "id": 135,
      "title": "Clever Chapter Title 111",
      "position": 3,
      "updated_at": "2016-10-18T16:44:16.687Z",
      "course_id": 252,
      "author_id": 757,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-18T16:44:16.326Z",
      "questions_updated_at": "2016-10-18T16:44:16.326Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 330d9d5729cdc7abe1cac1aa5d15db1a8c1832f8888a071fc684484e2ae39433"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0109e559d52c7d84fda9efd953b07d0ecad3512e0d193cf92d9c4edd4eceee35
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
      "id": 136,
      "title": "Clever Chapter Title 112",
      "position": 1,
      "updated_at": "2016-10-18T16:44:16.981Z",
      "course_id": 254,
      "author_id": 764,
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
      "id": 137,
      "title": "Clever Chapter Title 113",
      "position": 2,
      "updated_at": "2016-10-18T16:44:17.006Z",
      "course_id": 254,
      "author_id": 765,
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
      "id": 138,
      "title": "Clever Chapter Title 114",
      "position": 3,
      "updated_at": "2016-10-18T16:44:17.032Z",
      "course_id": 254,
      "author_id": 766,
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
	-H "Authorization: Bearer 0109e559d52c7d84fda9efd953b07d0ecad3512e0d193cf92d9c4edd4eceee35"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/173
Content-Type: application/json
Authorization: Bearer 5384d80f9423dc96d62de727209b4efab67c5e6aea8fe111b918844c0649180a
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/173" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5384d80f9423dc96d62de727209b4efab67c5e6aea8fe111b918844c0649180a"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2adc33d729369e110f4eb03bda011a0a5b85c308ee858cefe2c14cb95c976a0b
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
	-H "Authorization: Bearer 2adc33d729369e110f4eb03bda011a0a5b85c308ee858cefe2c14cb95c976a0b"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b4ed272e493d44bd3efea6938b50fadc9ffc770bb82c6f724df3ae59ceb0bb13
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
    "creator_id": 584,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 168,
    "additional_university_ids": [

    ],
    "topic_id": 193,
    "discipline_id": 193,
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
    "chapters_updated_at": "2016-10-18T16:44:02.768Z",
    "updated_at": "2016-10-18T16:44:04.232Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 119,
        "title": "Clever Chapter Title 98",
        "position": 1,
        "updated_at": "2016-10-18T16:44:04.180Z",
        "course_id": 183,
        "author_id": 584,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T16:44:02.768Z",
        "questions_updated_at": "2016-10-18T16:44:02.768Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 120,
        "title": "Clever Chapter Title 99",
        "position": 2,
        "updated_at": "2016-10-18T16:44:04.224Z",
        "course_id": 183,
        "author_id": 584,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-18T16:44:02.768Z",
        "questions_updated_at": "2016-10-18T16:44:02.768Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 584,
        "chapter_id": 119,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.012Z",
        "created_at": "2016-10-18T16:44:04.012Z",
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
        "author_id": 584,
        "chapter_id": 120,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.086Z",
        "created_at": "2016-10-18T16:44:04.086Z",
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
        "author_id": 584,
        "chapter_id": 119,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.052Z",
        "created_at": "2016-10-18T16:44:04.052Z",
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
        "author_id": 584,
        "chapter_id": 120,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.128Z",
        "created_at": "2016-10-18T16:44:04.128Z",
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
        "author_id": 587,
        "chapter_id": 119,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.170Z",
        "created_at": "2016-10-18T16:44:04.170Z",
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
        "author_id": 588,
        "chapter_id": 120,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T16:44:04.213Z",
        "created_at": "2016-10-18T16:44:04.213Z",
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
	-H "Authorization: Bearer b4ed272e493d44bd3efea6938b50fadc9ffc770bb82c6f724df3ae59ceb0bb13"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/188
Content-Type: application/json
Authorization: Bearer 33c4850c30e468004c87ef00dfee56329a7f8b259134d613dd6c3896a60df5d5
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
    "creator_id": 605,
    "id": 188,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 173,
    "additional_university_ids": [

    ],
    "topic_id": 198,
    "discipline_id": 198,
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
    "updated_at": "2016-10-18T16:44:07.784Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/188" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33c4850c30e468004c87ef00dfee56329a7f8b259134d613dd6c3896a60df5d5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0a13c3c6151307533cd101453dc8327678f0bc8001c2192243220a192b497741
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
    "creator_id": 610,
    "id": 191,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "topic_id": 201,
    "discipline_id": 201,
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
    "updated_at": "2016-10-18T16:44:08.165Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a13c3c6151307533cd101453dc8327678f0bc8001c2192243220a192b497741"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 0c4869843ea03c87d113a8e0f9b964317649e606957d2691fb3c2488015af6fd
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
      "id": 15,
      "user_id": 182,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:29.475Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 186,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:29.776Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 190,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:30.070Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 194,
      "feedbackable_id": 14,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:30.368Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 198,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T16:43:30.668Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c4869843ea03c87d113a8e0f9b964317649e606957d2691fb3c2488015af6fd"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer bee9d017bcb9ba7be6124afa8c2a16caeca898b38450600c4abd415d83eee133
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
      "id": 14,
      "user_id": 177,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-18T16:43:29.135Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bee9d017bcb9ba7be6124afa8c2a16caeca898b38450600c4abd415d83eee133"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Authorization: Bearer 9b018c0e60c8bc46f316eb8268501531d5dca9c49cadc4e0c630ef1e4593f71b
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
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Authorization: Bearer 9b018c0e60c8bc46f316eb8268501531d5dca9c49cadc4e0c630ef1e4593f71b" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer 3e17423d3acbdad79949b807a581c56ea84eeed4bb8c9e1b983696074dea0922
Content-Type: application/json
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
      "id": 117,
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
      "created_at": "2016-10-18T16:43:25.239Z",
      "updated_at": "2016-10-18T16:43:25.239Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-18T16:43:25.309Z",
    "updated_at": "2016-10-18T16:43:25.309Z",
    "course_id": 62,
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
	-H "Authorization: Bearer 3e17423d3acbdad79949b807a581c56ea84eeed4bb8c9e1b983696074dea0922" \
	-H "Content-Type: application/json"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/5/feedbacks
Content-Type: application/json
Authorization: Bearer 1fdeb848b5bfd6592952340f08dfc7983b7a963008b7b164c0b9ed246588a853
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
      "id": 2,
      "user_id": 79,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:23.260Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 1,
      "user_id": 78,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:23.248Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fdeb848b5bfd6592952340f08dfc7983b7a963008b7b164c0b9ed246588a853"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer a3dae2e926c48657f70f73d8ef2a36302e1896c632339277a03369ee7779e84c
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 385,
      "chapter_id": 73,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:42.691Z",
      "created_at": "2016-10-18T16:43:42.691Z",
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
      "id": 46,
      "obfuscated_id": "urkHiAaH08E",
      "author_id": 388,
      "chapter_id": 74,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:42.830Z",
      "created_at": "2016-10-18T16:43:42.830Z",
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
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 391,
      "chapter_id": 75,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:42.970Z",
      "created_at": "2016-10-18T16:43:42.970Z",
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
      "author_id": 394,
      "chapter_id": 76,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:43.109Z",
      "created_at": "2016-10-18T16:43:43.109Z",
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
      "author_id": 397,
      "chapter_id": 77,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:43.258Z",
      "created_at": "2016-10-18T16:43:43.258Z",
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
	-H "Authorization: Bearer a3dae2e926c48657f70f73d8ef2a36302e1896c632339277a03369ee7779e84c"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4fbcdea9e1bd6e24fd1276fe083fe6817d4a0e55ddb1889b301a38a80a0b7b94
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 413,
      "chapter_id": 82,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:43:44.116Z",
      "created_at": "2016-10-18T16:43:44.116Z",
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
	-H "Authorization: Bearer 4fbcdea9e1bd6e24fd1276fe083fe6817d4a0e55ddb1889b301a38a80a0b7b94"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/republish
Content-Type: application/json
Authorization: Bearer 91a55fbdd274b4f058a7d0a99aa12f403e08a581b9d656c0cefdaf9783d557b1
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
	-H "Authorization: Bearer 91a55fbdd274b4f058a7d0a99aa12f403e08a581b9d656c0cefdaf9783d557b1"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/51/feedbacks
Content-Type: application/json
Authorization: Bearer b9beaff6e8c81ad1ab67268fcde7589737d113c455dc266ae5c8e911714f985b
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
      "id": 40,
      "user_id": 508,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:54.991Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 507,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T16:43:54.979Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/51/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9beaff6e8c81ad1ab67268fcde7589737d113c455dc266ae5c8e911714f985b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer f4ccffd175d0b9672dfe081b6ab2d3f93eccdd6a9e69c726f3a85c7a744f887e
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
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 905,
      "chapter_id": 181,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:29.605Z",
      "created_at": "2016-10-18T16:44:29.486Z",
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
          "id": 249,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 250,
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
      "author_id": 896,
      "chapter_id": 178,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:28.718Z",
      "created_at": "2016-10-18T16:44:28.602Z",
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
    },
    {
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 899,
      "chapter_id": 179,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:29.001Z",
      "created_at": "2016-10-18T16:44:28.883Z",
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
          "id": 245,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 246,
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
      "author_id": 902,
      "chapter_id": 180,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:29.319Z",
      "created_at": "2016-10-18T16:44:29.200Z",
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
          "id": 247,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 248,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 908,
      "chapter_id": 182,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:29.893Z",
      "created_at": "2016-10-18T16:44:29.778Z",
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
          "id": 251,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 252,
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
	-H "Authorization: Bearer f4ccffd175d0b9672dfe081b6ab2d3f93eccdd6a9e69c726f3a85c7a744f887e"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 5f4d0b7915e0ee96b89668709756ee86a168141cf452a1a2ba0853fe94423e0a
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
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 876,
      "chapter_id": 172,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T16:44:26.874Z",
      "created_at": "2016-10-18T16:44:26.760Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f4d0b7915e0ee96b89668709756ee86a168141cf452a1a2ba0853fe94423e0a"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/108/republish
Content-Type: application/json
Authorization: Bearer 4b89627f09f2c5791e49e94f7e9ca40de7650c0e1e71d54883216ccc17c93716
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/108/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b89627f09f2c5791e49e94f7e9ca40de7650c0e1e71d54883216ccc17c93716"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cef1c81797724bb010e012f21bd3925ca06381102b663b0fb55c986b8d7d3bb8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":6,"published":false}}
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
    "creator_id": 14,
    "id": 6,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 6,
    "additional_university_ids": [

    ],
    "topic_id": 6,
    "discipline_id": 6,
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
    "updated_at": "2016-10-18T16:43:17.123Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":6,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cef1c81797724bb010e012f21bd3925ca06381102b663b0fb55c986b8d7d3bb8"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6dbfcca5654330175e14e0b139a1069cac08d1710a6b0f4c89064c2b05059885
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
      "creator_id": 21,
      "id": 13,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-9",
      "html_url": "https://goskive.com/course/fu-course-9",
      "slug": "fu-course-9",
      "university_id": 11,
      "additional_university_ids": [

      ],
      "topic_id": 13,
      "discipline_id": 13,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 9",
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
      "updated_at": "2016-10-18T16:43:17.887Z",
      "shortname": "fu-course-9"
    },
    {
      "creator_id": 21,
      "id": 14,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-10",
      "html_url": "https://goskive.com/course/fu-course-10",
      "slug": "fu-course-10",
      "university_id": 11,
      "additional_university_ids": [

      ],
      "topic_id": 14,
      "discipline_id": 14,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 10",
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
      "updated_at": "2016-10-18T16:43:17.928Z",
      "shortname": "fu-course-10"
    },
    {
      "creator_id": 22,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 11,
      "additional_university_ids": [

      ],
      "topic_id": 15,
      "discipline_id": 15,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
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
      "updated_at": "2016-10-18T16:43:17.977Z",
      "shortname": "fu-course-11"
    },
    {
      "creator_id": 22,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 11,
      "additional_university_ids": [

      ],
      "topic_id": 16,
      "discipline_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
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
      "chapters_updated_at": "2016-10-18T16:43:18.359Z",
      "updated_at": "2016-10-18T16:43:18.366Z",
      "shortname": "fu-course-12"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dbfcca5654330175e14e0b139a1069cac08d1710a6b0f4c89064c2b05059885"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ccd9d33fbf50d69cdcfe45627fd714a4df057ca455f52f6a7159c33bb40ff768
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
      "creator_id": 28,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-13",
      "html_url": "https://goskive.com/course/fu-course-13",
      "slug": "fu-course-13",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 17,
      "discipline_id": 17,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 13",
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
      "updated_at": "2016-10-18T16:43:18.569Z",
      "shortname": "fu-course-13"
    },
    {
      "creator_id": 28,
      "id": 18,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-14",
      "html_url": "https://goskive.com/course/fu-course-14",
      "slug": "fu-course-14",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 18,
      "discipline_id": 18,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 14",
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
      "updated_at": "2016-10-18T16:43:18.608Z",
      "shortname": "fu-course-14"
    },
    {
      "creator_id": 29,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 19,
      "discipline_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
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
      "updated_at": "2016-10-18T16:43:18.654Z",
      "shortname": "fu-course-15"
    },
    {
      "creator_id": 29,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
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
      "updated_at": "2016-10-18T16:43:18.693Z",
      "shortname": "fu-course-16"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccd9d33fbf50d69cdcfe45627fd714a4df057ca455f52f6a7159c33bb40ff768"
```
