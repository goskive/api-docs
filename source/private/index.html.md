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
DELETE /v2/chapters/102
Content-Type: application/json
Authorization: Bearer 6342ad4141569ce7008829e55b0d8558cdcaa55f228c87bbb0c1b4d74e5d3a88
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/102" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6342ad4141569ce7008829e55b0d8558cdcaa55f228c87bbb0c1b4d74e5d3a88"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/97
Content-Type: application/json
Authorization: Bearer 0fb2a44c2ba71893846324835e50ebb838fef606bf1a86dbc8d7230f05740f50
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
    "id": 97,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T18:40:51.302Z",
    "course_id": 207,
    "author_id": 587,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T18:40:50.775Z",
    "questions_updated_at": "2016-10-25T18:40:50.775Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 590,
        "chapter_id": 97,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:51.223Z",
        "created_at": "2016-10-25T18:40:51.223Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 591,
        "chapter_id": 97,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:51.286Z",
        "created_at": "2016-10-25T18:40:51.286Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 588,
        "chapter_id": 97,
        "position": 61,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:50.978Z",
        "created_at": "2016-10-25T18:40:50.875Z",
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
            "id": 140,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 141,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 589,
        "chapter_id": 97,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:51.158Z",
        "created_at": "2016-10-25T18:40:51.045Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/97" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fb2a44c2ba71893846324835e50ebb838fef606bf1a86dbc8d7230f05740f50"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/104
Content-Type: application/json
Authorization: Bearer 4af14463872924968a44d6ca6f6befe7dc8874558486f8413031afb2142551b2
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
    "id": 104,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T18:40:53.087Z",
    "course_id": 214,
    "author_id": 616,
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
curl "api.goskive.com/v2/chapters/104" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4af14463872924968a44d6ca6f6befe7dc8874558486f8413031afb2142551b2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/45
Content-Type: application/json
Authorization: Bearer beec0d81d194cb5ecd1716068570e688b577a91aebcb925c5357676f80e4373a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/45" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer beec0d81d194cb5ecd1716068570e688b577a91aebcb925c5357676f80e4373a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 1d2752ca55e12d9c53cc8176b515a26ebad329b50c19637de973473c9ad5e2ff
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
      "id": 16,
      "author_id": 427,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:40.064Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 429,
      "reply_to_id": 16,
      "created_at": "2016-10-25T18:40:40.144Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 431,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:40.225Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 433,
      "reply_to_id": 18,
      "created_at": "2016-10-25T18:40:40.305Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 435,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:40.385Z",
      "status": "reported",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 437,
      "reply_to_id": 20,
      "created_at": "2016-10-25T18:40:40.467Z",
      "status": "published",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 439,
      "reply_to_id": 20,
      "created_at": "2016-10-25T18:40:40.549Z",
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
	-H "Authorization: Bearer 1d2752ca55e12d9c53cc8176b515a26ebad329b50c19637de973473c9ad5e2ff"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer f86b1c70ab14a46fe5e7c5f013201ce710e25e698d43f85bd0f7012444c5ea5a
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
      "id": 23,
      "author_id": 442,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:40.684Z",
      "status": "published",
      "subject_id": 163,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 444,
      "reply_to_id": 23,
      "created_at": "2016-10-25T18:40:40.766Z",
      "status": "published",
      "subject_id": 164,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 446,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:40.850Z",
      "status": "published",
      "subject_id": 165,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 448,
      "reply_to_id": 25,
      "created_at": "2016-10-25T18:40:40.931Z",
      "status": "published",
      "subject_id": 166,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 450,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:41.042Z",
      "status": "reported",
      "subject_id": 167,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 452,
      "reply_to_id": 27,
      "created_at": "2016-10-25T18:40:41.123Z",
      "status": "published",
      "subject_id": 168,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 454,
      "reply_to_id": 27,
      "created_at": "2016-10-25T18:40:41.204Z",
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
	-H "Authorization: Bearer f86b1c70ab14a46fe5e7c5f013201ce710e25e698d43f85bd0f7012444c5ea5a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e00c687ae4a57c771d7bf271262175f3c40522419dc29f0815496c47d4d3b359
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
      "id": 31,
      "author_id": 459,
      "reply_to_id": 30,
      "created_at": "2016-10-25T18:40:41.415Z",
      "status": "published",
      "subject_id": 171,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 463,
      "reply_to_id": 32,
      "created_at": "2016-10-25T18:40:41.572Z",
      "status": "published",
      "subject_id": 173,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 467,
      "reply_to_id": 34,
      "created_at": "2016-10-25T18:40:41.732Z",
      "status": "published",
      "subject_id": 175,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 469,
      "reply_to_id": 34,
      "created_at": "2016-10-25T18:40:41.814Z",
      "status": "published",
      "subject_id": 176,
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
	-H "Authorization: Bearer e00c687ae4a57c771d7bf271262175f3c40522419dc29f0815496c47d4d3b359"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 9907f5e231f5b9fc454daf011fdfabffd8f39e99dd076c0d3f6eed9fcc98deab
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
      "id": 13,
      "author_id": 420,
      "reply_to_id": null,
      "created_at": "2016-10-25T18:40:39.774Z",
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
	-H "Authorization: Bearer 9907f5e231f5b9fc454daf011fdfabffd8f39e99dd076c0d3f6eed9fcc98deab"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/7/republish
Content-Type: application/json
Authorization: Bearer 93281b8b1d91a43aa1c6c0bb18735358503caefd5883e1913bcca98f61b4992b
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/7/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93281b8b1d91a43aa1c6c0bb18735358503caefd5883e1913bcca98f61b4992b"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/245/chapters
Content-Type: application/json
Authorization: Bearer 9db4cfbdca8b863c8891cb1385a62f06e47611e4e690e5c0da43e89e00d25f65
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
    "id": 127,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T18:41:04.067Z",
    "course_id": 245,
    "author_id": 709,
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
curl "api.goskive.com/v2/courses/245/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9db4cfbdca8b863c8891cb1385a62f06e47611e4e690e5c0da43e89e00d25f65"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c5fdc2df0c9bcd7e991e03881cb8aaf91b4f8541dc5e32bdbd7267675b2e62bd
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
    "id": 128,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T18:41:04.190Z",
    "course_id": 246,
    "author_id": 711,
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
	-H "Authorization: Bearer c5fdc2df0c9bcd7e991e03881cb8aaf91b4f8541dc5e32bdbd7267675b2e62bd"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 57b0df9c58f259e315516a4626e9cf66649f04f2ebb142c51b97c497f5bfa501
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
      "id": 130,
      "title": "Clever Chapter Title 115",
      "position": 1,
      "updated_at": "2016-10-25T18:41:04.543Z",
      "course_id": 249,
      "author_id": 717,
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
      "id": 131,
      "title": "Clever Chapter Title 116",
      "position": 2,
      "updated_at": "2016-10-25T18:41:04.566Z",
      "course_id": 249,
      "author_id": 718,
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
      "id": 132,
      "title": "Clever Chapter Title 117",
      "position": 3,
      "updated_at": "2016-10-25T18:41:04.810Z",
      "course_id": 249,
      "author_id": 719,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T18:41:04.472Z",
      "questions_updated_at": "2016-10-25T18:41:04.472Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57b0df9c58f259e315516a4626e9cf66649f04f2ebb142c51b97c497f5bfa501"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c3817d8677f6c953b4897e92ecb7cacc67387e4778346a2f68a4b3bf78d0a7b7
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
      "title": "Clever Chapter Title 118",
      "position": 1,
      "updated_at": "2016-10-25T18:41:05.046Z",
      "course_id": 251,
      "author_id": 726,
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
      "title": "Clever Chapter Title 119",
      "position": 2,
      "updated_at": "2016-10-25T18:41:05.069Z",
      "course_id": 251,
      "author_id": 727,
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
      "title": "Clever Chapter Title 120",
      "position": 3,
      "updated_at": "2016-10-25T18:41:05.092Z",
      "course_id": 251,
      "author_id": 728,
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
	-H "Authorization: Bearer c3817d8677f6c953b4897e92ecb7cacc67387e4778346a2f68a4b3bf78d0a7b7"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e05af36450e3fdafd51b391674f551420efdf437692ed0fcf8627d98167d4adc
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
	-H "Authorization: Bearer e05af36450e3fdafd51b391674f551420efdf437692ed0fcf8627d98167d4adc"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/232
Content-Type: application/json
Authorization: Bearer e9852e3516f81b6a96bc805eccf0068fd9e7e355a50a4034f8672e7eb97f1126
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/232" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9852e3516f81b6a96bc805eccf0068fd9e7e355a50a4034f8672e7eb97f1126"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 439658caa7f1fd7f7397800732b60b1243e80df994e4e603796414172f0e48d6
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
    "creator_id": 639,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "topic_id": 229,
    "discipline_id": 230,
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
    "chapters_updated_at": "2016-10-25T18:40:56.753Z",
    "updated_at": "2016-10-25T18:40:58.101Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 110,
        "title": "Clever Chapter Title 98",
        "position": 1,
        "updated_at": "2016-10-25T18:40:58.056Z",
        "course_id": 222,
        "author_id": 639,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T18:40:56.753Z",
        "questions_updated_at": "2016-10-25T18:40:56.753Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 111,
        "title": "Clever Chapter Title 99",
        "position": 2,
        "updated_at": "2016-10-25T18:40:58.094Z",
        "course_id": 222,
        "author_id": 639,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T18:40:56.753Z",
        "questions_updated_at": "2016-10-25T18:40:56.753Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 639,
        "chapter_id": 110,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:57.907Z",
        "created_at": "2016-10-25T18:40:57.907Z",
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
        "author_id": 639,
        "chapter_id": 111,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:57.974Z",
        "created_at": "2016-10-25T18:40:57.974Z",
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
        "author_id": 639,
        "chapter_id": 110,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:57.945Z",
        "created_at": "2016-10-25T18:40:57.945Z",
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
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 639,
        "chapter_id": 111,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:58.011Z",
        "created_at": "2016-10-25T18:40:58.011Z",
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
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 642,
        "chapter_id": 110,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:58.047Z",
        "created_at": "2016-10-25T18:40:58.047Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 643,
        "chapter_id": 111,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T18:40:58.084Z",
        "created_at": "2016-10-25T18:40:58.084Z",
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
	-H "Authorization: Bearer 439658caa7f1fd7f7397800732b60b1243e80df994e4e603796414172f0e48d6"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/216
Content-Type: application/json
Authorization: Bearer 5ae9f40059d6995667b009174bcf2ee22f3e830cbeb2d41711bae38fed3553d5
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
    "creator_id": 621,
    "id": 216,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 201,
    "additional_university_ids": [

    ],
    "topic_id": 223,
    "discipline_id": 224,
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
    "updated_at": "2016-10-25T18:40:53.437Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/216" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ae9f40059d6995667b009174bcf2ee22f3e830cbeb2d41711bae38fed3553d5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 54b8d2701ea10f340cdae9fcf228b720905febfa63dc78bbe6bdf99b578650ee
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
    "creator_id": 625,
    "id": 218,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 203,
    "additional_university_ids": [

    ],
    "topic_id": 225,
    "discipline_id": 226,
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
    "updated_at": "2016-10-25T18:40:53.667Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54b8d2701ea10f340cdae9fcf228b720905febfa63dc78bbe6bdf99b578650ee"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 0e20a80d9fdfe77ec48712baaa76427d207e1cca654d3195a5d9ebc9827ae324
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
      "user_id": 821,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:10.110Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 825,
      "feedbackable_id": 110,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:10.388Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 829,
      "feedbackable_id": 111,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:10.681Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 833,
      "feedbackable_id": 112,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:10.966Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 837,
      "feedbackable_id": 113,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T18:41:11.258Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e20a80d9fdfe77ec48712baaa76427d207e1cca654d3195a5d9ebc9827ae324"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 99919ea3b5ffc1c718a81ceedbecda1b45d64d136a5718c114cbfd155c968ea2
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
      "user_id": 895,
      "feedbackable_id": 127,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T18:41:15.465Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99919ea3b5ffc1c718a81ceedbecda1b45d64d136a5718c114cbfd155c968ea2"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 04cd65c77dc10e450916d66e4d60d5e39c146626d5725d0e6858a1fa88a2f8c8
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04cd65c77dc10e450916d66e4d60d5e39c146626d5725d0e6858a1fa88a2f8c8"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/4/metadata
Content-Type: application/json
Authorization: Bearer 83a9ec108492a1b8b48404c257458eaa1ff896179963f2cbb9581917d1da4e6a
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
    "id": 4,
    "uploader": {
      "id": 230,
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
      "created_at": "2016-10-25T18:40:23.922Z",
      "updated_at": "2016-10-25T18:40:23.922Z"
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
    "created_at": "2016-10-25T18:40:23.994Z",
    "updated_at": "2016-10-25T18:40:23.994Z",
    "course_id": 96,
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
curl "api.goskive.com/v2/files/4/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83a9ec108492a1b8b48404c257458eaa1ff896179963f2cbb9581917d1da4e6a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/87/feedbacks
Content-Type: application/json
Authorization: Bearer e73005f2af42ce93784e53f442d3296d949d75c785c42ec8acbfca89bcd792c3
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
      "id": 42,
      "user_id": 940,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:19.124Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 939,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:41:19.115Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e73005f2af42ce93784e53f442d3296d949d75c785c42ec8acbfca89bcd792c3"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 7a3e4ed6ce99e8e7ce82a18127d3dfb4ab25ce59c29de25ffeca7e5b0e754c3a
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 188,
      "chapter_id": 39,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.401Z",
      "created_at": "2016-10-25T18:40:21.401Z",
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
      "author_id": 191,
      "chapter_id": 40,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.522Z",
      "created_at": "2016-10-25T18:40:21.522Z",
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 194,
      "chapter_id": 41,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.645Z",
      "created_at": "2016-10-25T18:40:21.645Z",
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 197,
      "chapter_id": 42,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.773Z",
      "created_at": "2016-10-25T18:40:21.773Z",
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 200,
      "chapter_id": 43,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.899Z",
      "created_at": "2016-10-25T18:40:21.899Z",
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
	-H "Authorization: Bearer 7a3e4ed6ce99e8e7ce82a18127d3dfb4ab25ce59c29de25ffeca7e5b0e754c3a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 9a1172f45230ac1f91aaca3f05083d4ea77524df97555d38fa0de608bf7fd4c5
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 184,
      "chapter_id": 38,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:21.228Z",
      "created_at": "2016-10-25T18:40:21.228Z",
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
	-H "Authorization: Bearer 9a1172f45230ac1f91aaca3f05083d4ea77524df97555d38fa0de608bf7fd4c5"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/32/republish
Content-Type: application/json
Authorization: Bearer 0b44e5839bcf732098d237c5911aaf9276e3e245a371134d997a8085a90f9ff4
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/32/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b44e5839bcf732098d237c5911aaf9276e3e245a371134d997a8085a90f9ff4"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/6/feedbacks
Content-Type: application/json
Authorization: Bearer 85adb6a9360315f76d6ab482530fadf981617c3b537273538c3cb5589a9b6394
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
      "user_id": 60,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:40:10.973Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 59,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T18:40:10.963Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/6/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85adb6a9360315f76d6ab482530fadf981617c3b537273538c3cb5589a9b6394"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 75cf3ba3145b3779c98ae3d9c996b42f891b5fdd981be62005cbdbaee9c23cd0
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 297,
      "chapter_id": 58,
      "position": 28,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:29.393Z",
      "created_at": "2016-10-25T18:40:29.283Z",
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 294,
      "chapter_id": 57,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:29.135Z",
      "created_at": "2016-10-25T18:40:29.021Z",
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
          "id": 60,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 61,
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
      "author_id": 300,
      "chapter_id": 59,
      "position": 29,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:29.662Z",
      "created_at": "2016-10-25T18:40:29.548Z",
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
      "author_id": 303,
      "chapter_id": 60,
      "position": 30,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:29.928Z",
      "created_at": "2016-10-25T18:40:29.815Z",
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 306,
      "chapter_id": 61,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:30.187Z",
      "created_at": "2016-10-25T18:40:30.081Z",
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75cf3ba3145b3779c98ae3d9c996b42f891b5fdd981be62005cbdbaee9c23cd0"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9bed4081f5aa72145fe083b8c7e28cc1456c9829eb3283566e8cfaa01f55e917
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
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 338,
      "chapter_id": 71,
      "position": 41,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T18:40:32.921Z",
      "created_at": "2016-10-25T18:40:32.814Z",
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
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bed4081f5aa72145fe083b8c7e28cc1456c9829eb3283566e8cfaa01f55e917"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/47/republish
Content-Type: application/json
Authorization: Bearer 9e913a6b3cdc6892e15cc7fb4886404b529607c0c9992dec7d90ec9bad82e554
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/47/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e913a6b3cdc6892e15cc7fb4886404b529607c0c9992dec7d90ec9bad82e554"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9f054c86da6fbd7aa61165fd0a53fb809eae3a31a8ef89de3ee2f538486ff5b2
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":67,"published":false}}
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
    "creator_id": 141,
    "id": 65,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 45,
    "additional_university_ids": [

    ],
    "topic_id": 67,
    "discipline_id": 67,
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
    "updated_at": "2016-10-25T18:40:19.028Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":67,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f054c86da6fbd7aa61165fd0a53fb809eae3a31a8ef89de3ee2f538486ff5b2"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 811f4dc240dac2b693814e1829e645e0bcff639ed4a7b6b320d06a5ca85afbae
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
      "creator_id": 131,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-53",
      "html_url": "https://goskive.com/course/fu-course-53",
      "slug": "fu-course-53",
      "university_id": 42,
      "additional_university_ids": [

      ],
      "topic_id": 59,
      "discipline_id": 59,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 53",
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
      "updated_at": "2016-10-25T18:40:18.201Z",
      "shortname": "fu-course-53"
    },
    {
      "creator_id": 131,
      "id": 58,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-54",
      "html_url": "https://goskive.com/course/fu-course-54",
      "slug": "fu-course-54",
      "university_id": 42,
      "additional_university_ids": [

      ],
      "topic_id": 60,
      "discipline_id": 60,
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
      "updated_at": "2016-10-25T18:40:18.236Z",
      "shortname": "fu-course-54"
    },
    {
      "creator_id": 132,
      "id": 59,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-55",
      "html_url": "https://goskive.com/course/fu-course-55",
      "slug": "fu-course-55",
      "university_id": 42,
      "additional_university_ids": [

      ],
      "topic_id": 61,
      "discipline_id": 61,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T18:40:18.277Z",
      "shortname": "fu-course-55"
    },
    {
      "creator_id": 132,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-56",
      "html_url": "https://goskive.com/course/fu-course-56",
      "slug": "fu-course-56",
      "university_id": 42,
      "additional_university_ids": [

      ],
      "topic_id": 62,
      "discipline_id": 62,
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
      "chapters_updated_at": "2016-10-25T18:40:18.573Z",
      "updated_at": "2016-10-25T18:40:18.579Z",
      "shortname": "fu-course-56"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 811f4dc240dac2b693814e1829e645e0bcff639ed4a7b6b320d06a5ca85afbae"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7ed554c3aa11685f14c52d5a704f68b5ccdc3629cde8493e253e6de2d3a68070
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
      "creator_id": 137,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 63,
      "discipline_id": 63,
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
      "updated_at": "2016-10-25T18:40:18.711Z",
      "shortname": "fu-course-57"
    },
    {
      "creator_id": 137,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 64,
      "discipline_id": 64,
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
      "updated_at": "2016-10-25T18:40:18.745Z",
      "shortname": "fu-course-58"
    },
    {
      "creator_id": 138,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 65,
      "discipline_id": 65,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T18:40:18.787Z",
      "shortname": "fu-course-59"
    },
    {
      "creator_id": 138,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-60",
      "html_url": "https://goskive.com/course/fu-course-60",
      "slug": "fu-course-60",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 66,
      "discipline_id": 66,
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
      "updated_at": "2016-10-25T18:40:18.822Z",
      "shortname": "fu-course-60"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ed554c3aa11685f14c52d5a704f68b5ccdc3629cde8493e253e6de2d3a68070"
```
