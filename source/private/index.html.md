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
DELETE /v2/chapters/181
Content-Type: application/json
Authorization: Bearer e32ec1ad86733e42ad111932b6277a504d37ea157be3e0a17f2d8153d5530770
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/181" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e32ec1ad86733e42ad111932b6277a504d37ea157be3e0a17f2d8153d5530770"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/176
Content-Type: application/json
Authorization: Bearer 9e27e9295f9890b6aaeacbd6af10a87c66f0678e1a5437bcac166e74d6785816
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
    "id": 176,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T17:13:27.602Z",
    "course_id": 290,
    "author_id": 888,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T17:13:27.106Z",
    "questions_updated_at": "2016-10-25T17:13:27.106Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 891,
        "chapter_id": 176,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:27.552Z",
        "created_at": "2016-10-25T17:13:27.552Z",
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
        "author_id": 892,
        "chapter_id": 176,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:27.586Z",
        "created_at": "2016-10-25T17:13:27.586Z",
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
        "id": 114,
        "obfuscated_id": "RwCVsRO9fcs",
        "author_id": 889,
        "chapter_id": 176,
        "position": 105,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:27.309Z",
        "created_at": "2016-10-25T17:13:27.207Z",
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
            "id": 228,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 229,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 890,
        "chapter_id": 176,
        "position": 106,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:27.486Z",
        "created_at": "2016-10-25T17:13:27.375Z",
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
            "id": 230,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 231,
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
curl "api.goskive.com/v2/chapters/176" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e27e9295f9890b6aaeacbd6af10a87c66f0678e1a5437bcac166e74d6785816"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/173
Content-Type: application/json
Authorization: Bearer d30baf1c939af4d96e2b32cfc52a0b558df0e8a56a1718b6a24d168f81fffe69
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
    "id": 173,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T17:13:26.822Z",
    "course_id": 287,
    "author_id": 880,
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
curl "api.goskive.com/v2/chapters/173" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d30baf1c939af4d96e2b32cfc52a0b558df0e8a56a1718b6a24d168f81fffe69"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/51
Content-Type: application/json
Authorization: Bearer 806cc422e8a06fe6341220fa5eef32793e9145121cd3365c32a33ae740c4eae0
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 806cc422e8a06fe6341220fa5eef32793e9145121cd3365c32a33ae740c4eae0"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5bc0d158300447a564544602d69537455a6ddc09d72249c02abefe126d71d487
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
      "author_id": 702,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:13.619Z",
      "status": "published",
      "subject_id": 200,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 704,
      "reply_to_id": 21,
      "created_at": "2016-10-25T17:13:13.695Z",
      "status": "published",
      "subject_id": 201,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 706,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:13.774Z",
      "status": "published",
      "subject_id": 202,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 708,
      "reply_to_id": 23,
      "created_at": "2016-10-25T17:13:13.854Z",
      "status": "published",
      "subject_id": 203,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 710,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:13.962Z",
      "status": "reported",
      "subject_id": 204,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 712,
      "reply_to_id": 25,
      "created_at": "2016-10-25T17:13:14.043Z",
      "status": "published",
      "subject_id": 205,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 714,
      "reply_to_id": 25,
      "created_at": "2016-10-25T17:13:14.122Z",
      "status": "published",
      "subject_id": 206,
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
	-H "Authorization: Bearer 5bc0d158300447a564544602d69537455a6ddc09d72249c02abefe126d71d487"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer ad45ebca5962b16dde6a130c72b23ec3e1e0c7f8ffe252c3eeed06f22d9d6b7a
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
      "author_id": 747,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:15.465Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 749,
      "reply_to_id": 42,
      "created_at": "2016-10-25T17:13:15.544Z",
      "status": "published",
      "subject_id": 222,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 751,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:15.622Z",
      "status": "published",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 753,
      "reply_to_id": 44,
      "created_at": "2016-10-25T17:13:15.701Z",
      "status": "published",
      "subject_id": 224,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 755,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:15.779Z",
      "status": "reported",
      "subject_id": 225,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 757,
      "reply_to_id": 46,
      "created_at": "2016-10-25T17:13:15.858Z",
      "status": "published",
      "subject_id": 226,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 759,
      "reply_to_id": 46,
      "created_at": "2016-10-25T17:13:15.939Z",
      "status": "published",
      "subject_id": 227,
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
	-H "Authorization: Bearer ad45ebca5962b16dde6a130c72b23ec3e1e0c7f8ffe252c3eeed06f22d9d6b7a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e43a6a20848c7f5fe71fcdf2755ba8b62fabf12408a6bff66343a719ae1e5e15
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
      "id": 36,
      "author_id": 734,
      "reply_to_id": 35,
      "created_at": "2016-10-25T17:13:14.944Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 738,
      "reply_to_id": 37,
      "created_at": "2016-10-25T17:13:15.105Z",
      "status": "published",
      "subject_id": 217,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 742,
      "reply_to_id": 39,
      "created_at": "2016-10-25T17:13:15.261Z",
      "status": "published",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 744,
      "reply_to_id": 39,
      "created_at": "2016-10-25T17:13:15.340Z",
      "status": "published",
      "subject_id": 220,
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
	-H "Authorization: Bearer e43a6a20848c7f5fe71fcdf2755ba8b62fabf12408a6bff66343a719ae1e5e15"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer ea29703541ad72efd1b531d3bfbba405ff06210eea6660837dc03e4192296c7c
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
      "id": 18,
      "author_id": 695,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:13.339Z",
      "status": "reported",
      "subject_id": 197,
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
	-H "Authorization: Bearer ea29703541ad72efd1b531d3bfbba405ff06210eea6660837dc03e4192296c7c"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/52/republish
Content-Type: application/json
Authorization: Bearer f660a863d35f5ff41ae9782bd51c514304c592bfad68edc4dd9d6dfa7a0a6019
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f660a863d35f5ff41ae9782bd51c514304c592bfad68edc4dd9d6dfa7a0a6019"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/156/chapters
Content-Type: application/json
Authorization: Bearer b760e6b86b6a028bb26d40d0f04683686d23c87c673a17debe6e980b25f5e7d3
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
    "updated_at": "2016-10-25T17:13:01.892Z",
    "course_id": 156,
    "author_id": 589,
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
curl "api.goskive.com/v2/courses/156/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b760e6b86b6a028bb26d40d0f04683686d23c87c673a17debe6e980b25f5e7d3"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 14dcbd877a609e6f94eb184d6925b8755ae3e1f9fd0b7773ab255011f989ebb6
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
    "id": 141,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T17:13:02.271Z",
    "course_id": 159,
    "author_id": 595,
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
	-H "Authorization: Bearer 14dcbd877a609e6f94eb184d6925b8755ae3e1f9fd0b7773ab255011f989ebb6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 65fca9c7fee19b2496296f52656785365435c19895f4164709c0231a242db66e
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
      "title": "Clever Chapter Title 130",
      "position": 1,
      "updated_at": "2016-10-25T17:13:01.183Z",
      "course_id": 153,
      "author_id": 575,
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
      "title": "Clever Chapter Title 131",
      "position": 2,
      "updated_at": "2016-10-25T17:13:01.209Z",
      "course_id": 153,
      "author_id": 576,
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
      "title": "Clever Chapter Title 132",
      "position": 3,
      "updated_at": "2016-10-25T17:13:01.455Z",
      "course_id": 153,
      "author_id": 577,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T17:13:01.108Z",
      "questions_updated_at": "2016-10-25T17:13:01.108Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65fca9c7fee19b2496296f52656785365435c19895f4164709c0231a242db66e"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 471a1a0a3f2648f0d86e817d115e8686f614bb96acb73c3577ba96a3d3d621af
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
      "title": "Clever Chapter Title 133",
      "position": 1,
      "updated_at": "2016-10-25T17:13:01.689Z",
      "course_id": 155,
      "author_id": 584,
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
      "title": "Clever Chapter Title 134",
      "position": 2,
      "updated_at": "2016-10-25T17:13:01.711Z",
      "course_id": 155,
      "author_id": 585,
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
      "title": "Clever Chapter Title 135",
      "position": 3,
      "updated_at": "2016-10-25T17:13:01.734Z",
      "course_id": 155,
      "author_id": 586,
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
	-H "Authorization: Bearer 471a1a0a3f2648f0d86e817d115e8686f614bb96acb73c3577ba96a3d3d621af"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/172
Content-Type: application/json
Authorization: Bearer 79de4867df9c99a840d679b365bf25038613d897d58f9ee68eb2b25fd55c96d4
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/172" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79de4867df9c99a840d679b365bf25038613d897d58f9ee68eb2b25fd55c96d4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b6caa4be1f5bfb643315aea14d9829e5d56202362d147e76f11f138457114c22
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
	-H "Authorization: Bearer b6caa4be1f5bfb643315aea14d9829e5d56202362d147e76f11f138457114c22"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer dd5843517a029badfed2e6b0817afe18b2f6d671a891891717c26cefc6feff6f
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
    "creator_id": 607,
    "id": 165,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 172,
    "additional_university_ids": [

    ],
    "topic_id": 167,
    "discipline_id": 167,
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
    "chapters_updated_at": "2016-10-25T17:13:04.185Z",
    "updated_at": "2016-10-25T17:13:05.551Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 144,
        "title": "Clever Chapter Title 138",
        "position": 1,
        "updated_at": "2016-10-25T17:13:05.505Z",
        "course_id": 165,
        "author_id": 607,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T17:13:04.185Z",
        "questions_updated_at": "2016-10-25T17:13:04.185Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 145,
        "title": "Clever Chapter Title 139",
        "position": 2,
        "updated_at": "2016-10-25T17:13:05.544Z",
        "course_id": 165,
        "author_id": 607,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T17:13:04.185Z",
        "questions_updated_at": "2016-10-25T17:13:04.185Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 607,
        "chapter_id": 144,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.354Z",
        "created_at": "2016-10-25T17:13:05.354Z",
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
        "author_id": 607,
        "chapter_id": 145,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.420Z",
        "created_at": "2016-10-25T17:13:05.420Z",
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
        "author_id": 607,
        "chapter_id": 144,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.391Z",
        "created_at": "2016-10-25T17:13:05.391Z",
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
        "author_id": 607,
        "chapter_id": 145,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.458Z",
        "created_at": "2016-10-25T17:13:05.458Z",
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
        "author_id": 610,
        "chapter_id": 144,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.496Z",
        "created_at": "2016-10-25T17:13:05.496Z",
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
        "author_id": 611,
        "chapter_id": 145,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.534Z",
        "created_at": "2016-10-25T17:13:05.534Z",
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
	-H "Authorization: Bearer dd5843517a029badfed2e6b0817afe18b2f6d671a891891717c26cefc6feff6f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/168
Content-Type: application/json
Authorization: Bearer b56f4f177e1f5b1fb4489b8a10f9e1c01f263bffd74dcf873f8ee928abae7ed6
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
    "creator_id": 624,
    "id": 168,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "topic_id": 170,
    "discipline_id": 170,
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
    "updated_at": "2016-10-25T17:13:08.726Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/168" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b56f4f177e1f5b1fb4489b8a10f9e1c01f263bffd74dcf873f8ee928abae7ed6"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e4e71111ee4558f5616256d390605dc883c2b9340808db7baccbbcbdb7180fa3
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
    "creator_id": 626,
    "id": 169,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "topic_id": 171,
    "discipline_id": 171,
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
    "updated_at": "2016-10-25T17:13:08.860Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4e71111ee4558f5616256d390605dc883c2b9340808db7baccbbcbdb7180fa3"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 70faa889be6639bdca270663f88eaaa858e8bfc7fbb067e5e27d1fdff017653f
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
      "user_id": 335,
      "feedbackable_id": 43,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:46.120Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 339,
      "feedbackable_id": 44,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:46.392Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 343,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:46.683Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 347,
      "feedbackable_id": 46,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:46.957Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 351,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T17:12:47.237Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70faa889be6639bdca270663f88eaaa858e8bfc7fbb067e5e27d1fdff017653f"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer bc6c0f8e8dcf1a188dc56b7613793da0395cea091b230f820b27a7e16ce044b9
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
      "id": 18,
      "user_id": 372,
      "feedbackable_id": 52,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T17:12:48.674Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc6c0f8e8dcf1a188dc56b7613793da0395cea091b230f820b27a7e16ce044b9"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer 607ae38782a4bffde6d55d3ad385646d3327442f71ce608a25513127e7f8c679
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 607ae38782a4bffde6d55d3ad385646d3327442f71ce608a25513127e7f8c679"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 35ac3c01da485c61273f3c73a09097d6d0590b3349baa5d84e1ccee243fed3d7
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
      "id": 488,
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
      "created_at": "2016-10-25T17:12:55.627Z",
      "updated_at": "2016-10-25T17:12:55.627Z"
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
    "created_at": "2016-10-25T17:12:55.698Z",
    "updated_at": "2016-10-25T17:12:55.698Z",
    "course_id": 129,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35ac3c01da485c61273f3c73a09097d6d0590b3349baa5d84e1ccee243fed3d7"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/7/feedbacks
Content-Type: application/json
Authorization: Bearer 1bd14c2488c68638e9c3c98221af3a7de9bc29be5312cc7ec7582bd9f29ae961
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
      "id": 8,
      "user_id": 61,
      "feedbackable_id": 7,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:23.738Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 60,
      "feedbackable_id": 7,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:23.727Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/7/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bd14c2488c68638e9c3c98221af3a7de9bc29be5312cc7ec7582bd9f29ae961"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer ca1e304be447ff7fb28ee870d50002b0b3597ccc32d7ae53526d0b84c0ca857c
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 246,
      "chapter_id": 52,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:41.191Z",
      "created_at": "2016-10-25T17:12:41.191Z",
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 249,
      "chapter_id": 53,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:41.322Z",
      "created_at": "2016-10-25T17:12:41.322Z",
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 252,
      "chapter_id": 54,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:41.458Z",
      "created_at": "2016-10-25T17:12:41.458Z",
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 255,
      "chapter_id": 55,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:41.616Z",
      "created_at": "2016-10-25T17:12:41.616Z",
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
      "id": 23,
      "obfuscated_id": "eUsQCUPDncM",
      "author_id": 258,
      "chapter_id": 56,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:41.748Z",
      "created_at": "2016-10-25T17:12:41.748Z",
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
	-H "Authorization: Bearer ca1e304be447ff7fb28ee870d50002b0b3597ccc32d7ae53526d0b84c0ca857c"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 16bf04279c348d37393bd575cfcfed97e119dde66aa5f088541f58df8e5bf3a3
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 290,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:43.219Z",
      "created_at": "2016-10-25T17:12:43.219Z",
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
	-H "Authorization: Bearer 16bf04279c348d37393bd575cfcfed97e119dde66aa5f088541f58df8e5bf3a3"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/republish
Content-Type: application/json
Authorization: Bearer ceab06878256c28c45b790787f3cc05a9cbf8a4f9f26377bd247e853f714fa1b
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceab06878256c28c45b790787f3cc05a9cbf8a4f9f26377bd247e853f714fa1b"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/130/feedbacks
Content-Type: application/json
Authorization: Bearer a99a34f22cbec9e726305b1511558394311341bd4205e728b92dfa25e93e1ebd
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
      "id": 42,
      "user_id": 955,
      "feedbackable_id": 130,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:13:32.645Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 954,
      "feedbackable_id": 130,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:13:32.636Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/130/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a99a34f22cbec9e726305b1511558394311341bd4205e728b92dfa25e93e1ebd"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 7613e9365387e93820f9bd6a5f0a9f795f8346b13838ae1b0d8697d743c8eb4b
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 163,
      "chapter_id": 33,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:33.715Z",
      "created_at": "2016-10-25T17:12:33.586Z",
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
          "id": 56,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 57,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 154,
      "chapter_id": 30,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:32.852Z",
      "created_at": "2016-10-25T17:12:32.729Z",
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
          "id": 50,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 51,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 157,
      "chapter_id": 31,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:33.139Z",
      "created_at": "2016-10-25T17:12:33.010Z",
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
          "id": 52,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 53,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 160,
      "chapter_id": 32,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:33.427Z",
      "created_at": "2016-10-25T17:12:33.298Z",
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
          "id": 54,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 55,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 166,
      "chapter_id": 34,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:34.001Z",
      "created_at": "2016-10-25T17:12:33.878Z",
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
          "id": 58,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 59,
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
	-H "Authorization: Bearer 7613e9365387e93820f9bd6a5f0a9f795f8346b13838ae1b0d8697d743c8eb4b"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 8c90bc750bbfaa5c1ffef5de246893c8a298590ccc93721babf713b970275fbc
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
      "author_id": 182,
      "chapter_id": 39,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:35.530Z",
      "created_at": "2016-10-25T17:12:35.408Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c90bc750bbfaa5c1ffef5de246893c8a298590ccc93721babf713b970275fbc"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/15/republish
Content-Type: application/json
Authorization: Bearer 126e81ca765a32ca0a31218d2f02ff04edc9bf1052c63dcf6467b4e32487820c
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/15/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 126e81ca765a32ca0a31218d2f02ff04edc9bf1052c63dcf6467b4e32487820c"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 790d0277730ac9ee1b7bf01155ee865f749b18daaacf120c4f70b177c7ad3600
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":249,"published":false}}
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
    "creator_id": 797,
    "id": 239,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 246,
    "additional_university_ids": [

    ],
    "topic_id": 249,
    "discipline_id": 249,
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
    "updated_at": "2016-10-25T17:13:19.129Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":249,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 790d0277730ac9ee1b7bf01155ee865f749b18daaacf120c4f70b177c7ad3600"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 361ddbec634ef0e5181fc9b2dc413460141d30d2ad2cbf33cee5789799acf830
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
      "creator_id": 831,
      "id": 270,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-213",
      "html_url": "https://goskive.com/course/fu-course-213",
      "slug": "fu-course-213",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 280,
      "discipline_id": 280,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 213",
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
      "updated_at": "2016-10-25T17:13:22.251Z",
      "shortname": "fu-course-213"
    },
    {
      "creator_id": 831,
      "id": 271,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 281,
      "discipline_id": 281,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
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
      "updated_at": "2016-10-25T17:13:22.289Z",
      "shortname": "fu-course-214"
    },
    {
      "creator_id": 832,
      "id": 272,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 282,
      "discipline_id": 282,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
      "updated_at": "2016-10-25T17:13:22.334Z",
      "shortname": "fu-course-215"
    },
    {
      "creator_id": 832,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-216",
      "html_url": "https://goskive.com/course/fu-course-216",
      "slug": "fu-course-216",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 283,
      "discipline_id": 283,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 216",
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
      "chapters_updated_at": "2016-10-25T17:13:22.604Z",
      "updated_at": "2016-10-25T17:13:22.610Z",
      "shortname": "fu-course-216"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 361ddbec634ef0e5181fc9b2dc413460141d30d2ad2cbf33cee5789799acf830"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5ee70c2b654a0311ca43ef820a31c01b1b2b9f41587eeb1cd4cab913cfc4916a
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
      "creator_id": 838,
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-217",
      "html_url": "https://goskive.com/course/fu-course-217",
      "slug": "fu-course-217",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 284,
      "discipline_id": 284,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 217",
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
      "updated_at": "2016-10-25T17:13:22.834Z",
      "shortname": "fu-course-217"
    },
    {
      "creator_id": 838,
      "id": 275,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-218",
      "html_url": "https://goskive.com/course/fu-course-218",
      "slug": "fu-course-218",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 285,
      "discipline_id": 285,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 218",
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
      "updated_at": "2016-10-25T17:13:22.870Z",
      "shortname": "fu-course-218"
    },
    {
      "creator_id": 839,
      "id": 276,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-219",
      "html_url": "https://goskive.com/course/fu-course-219",
      "slug": "fu-course-219",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 286,
      "discipline_id": 286,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 219",
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
      "updated_at": "2016-10-25T17:13:22.914Z",
      "shortname": "fu-course-219"
    },
    {
      "creator_id": 839,
      "id": 277,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-220",
      "html_url": "https://goskive.com/course/fu-course-220",
      "slug": "fu-course-220",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 287,
      "discipline_id": 287,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 220",
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
      "updated_at": "2016-10-25T17:13:22.951Z",
      "shortname": "fu-course-220"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ee70c2b654a0311ca43ef820a31c01b1b2b9f41587eeb1cd4cab913cfc4916a"
```
