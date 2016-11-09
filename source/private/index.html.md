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
DELETE /v2/chapters/160
Content-Type: application/json
Authorization: Bearer a417ae12df5a32ea52bb485c8f30d8614b5221a15f7da3574aea037b9425dd83
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/160" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a417ae12df5a32ea52bb485c8f30d8614b5221a15f7da3574aea037b9425dd83"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/164
Content-Type: application/json
Authorization: Bearer 2a5e785e8c1dbbdd6a8e9315aeb9ed09ee3016f6ac9d2a94992506f713da645f
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
    "id": 164,
    "updated_at": "2016-11-09T11:19:09.520Z",
    "course_id": 239,
    "author_id": 743,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-09T11:19:08.926Z",
    "questions_updated_at": "2016-11-09T11:19:08.926Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 746,
        "chapter_id": 164,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:09.460Z",
        "created_at": "2016-11-09T11:19:09.460Z",
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
        "author_id": 747,
        "chapter_id": 164,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:09.501Z",
        "created_at": "2016-11-09T11:19:09.501Z",
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
        "author_id": 744,
        "chapter_id": 164,
        "position": 101,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:09.168Z",
        "created_at": "2016-11-09T11:19:09.045Z",
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
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 745,
        "chapter_id": 164,
        "position": 102,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:09.384Z",
        "created_at": "2016-11-09T11:19:09.247Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/164" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a5e785e8c1dbbdd6a8e9315aeb9ed09ee3016f6ac9d2a94992506f713da645f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/165
Content-Type: application/json
Authorization: Bearer fcc933bf8fc4fe46b4a6d400beec237bcad1390a9f258844196cb775ef92f9f8
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
    "id": 165,
    "updated_at": "2016-11-09T11:19:09.751Z",
    "course_id": 240,
    "author_id": 750,
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
curl "api.goskive.com/v2/chapters/165" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcc933bf8fc4fe46b4a6d400beec237bcad1390a9f258844196cb775ef92f9f8"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/25
Content-Type: application/json
Authorization: Bearer 4f859e36b60e8f14306596dc826949f17a346ad4e090b42369662cccc51d6549
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/25" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f859e36b60e8f14306596dc826949f17a346ad4e090b42369662cccc51d6549"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer ab74457ef62df66e8a74cf927c4d32d2865d8cf2ddab2e9989250a555221b524
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
      "id": 26,
      "author_id": 915,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:21.124Z",
      "status": "published",
      "subject_id": 282,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 917,
      "reply_to_id": 26,
      "created_at": "2016-11-09T11:19:21.214Z",
      "status": "published",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 919,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:21.306Z",
      "status": "published",
      "subject_id": 284,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 921,
      "reply_to_id": 28,
      "created_at": "2016-11-09T11:19:21.397Z",
      "status": "published",
      "subject_id": 285,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 923,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:21.489Z",
      "status": "reported",
      "subject_id": 286,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 925,
      "reply_to_id": 30,
      "created_at": "2016-11-09T11:19:21.581Z",
      "status": "published",
      "subject_id": 287,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 927,
      "reply_to_id": 30,
      "created_at": "2016-11-09T11:19:21.675Z",
      "status": "published",
      "subject_id": 288,
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
	-H "Authorization: Bearer ab74457ef62df66e8a74cf927c4d32d2865d8cf2ddab2e9989250a555221b524"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 7167e9b6f049550ed48085c51ed984e5f5bd912215f101e9ca0432945a87ef9e
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
      "author_id": 930,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:21.826Z",
      "status": "published",
      "subject_id": 289,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 932,
      "reply_to_id": 33,
      "created_at": "2016-11-09T11:19:21.918Z",
      "status": "published",
      "subject_id": 290,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 934,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:22.009Z",
      "status": "published",
      "subject_id": 291,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 936,
      "reply_to_id": 35,
      "created_at": "2016-11-09T11:19:22.100Z",
      "status": "published",
      "subject_id": 292,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 938,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:22.193Z",
      "status": "reported",
      "subject_id": 293,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 940,
      "reply_to_id": 37,
      "created_at": "2016-11-09T11:19:22.288Z",
      "status": "published",
      "subject_id": 294,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 942,
      "reply_to_id": 37,
      "created_at": "2016-11-09T11:19:22.417Z",
      "status": "published",
      "subject_id": 295,
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
	-H "Authorization: Bearer 7167e9b6f049550ed48085c51ed984e5f5bd912215f101e9ca0432945a87ef9e"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e1817405d34befb2efb5644d5762b356fa7174e6b9796f92d0a216653c86f25f
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
      "id": 48,
      "author_id": 962,
      "reply_to_id": 47,
      "created_at": "2016-11-09T11:19:23.392Z",
      "status": "published",
      "subject_id": 304,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 966,
      "reply_to_id": 49,
      "created_at": "2016-11-09T11:19:23.584Z",
      "status": "published",
      "subject_id": 306,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 970,
      "reply_to_id": 51,
      "created_at": "2016-11-09T11:19:23.758Z",
      "status": "published",
      "subject_id": 308,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 972,
      "reply_to_id": 51,
      "created_at": "2016-11-09T11:19:23.846Z",
      "status": "published",
      "subject_id": 309,
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
	-H "Authorization: Bearer e1817405d34befb2efb5644d5762b356fa7174e6b9796f92d0a216653c86f25f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 5d447e46ee04b7e979a3b7db5b258b2a90ef97d92019bae0b896757b2c3481c2
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
      "id": 58,
      "author_id": 983,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:19:24.339Z",
      "status": "reported",
      "subject_id": 314,
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
	-H "Authorization: Bearer 5d447e46ee04b7e979a3b7db5b258b2a90ef97d92019bae0b896757b2c3481c2"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer f992e8d50c46107b2ac19be20d2b6c69daf121b7cc735c4120dd7644e084dbc3
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f992e8d50c46107b2ac19be20d2b6c69daf121b7cc735c4120dd7644e084dbc3"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/194/chapters
Content-Type: application/json
Authorization: Bearer 52130784ea8bc22031b20ba5d83090245c127ae1bbd9ff2147a0ffe8899baff1
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
    "updated_at": "2016-11-09T11:18:48.116Z",
    "course_id": 194,
    "author_id": 590,
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
curl "api.goskive.com/v2/courses/194/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52130784ea8bc22031b20ba5d83090245c127ae1bbd9ff2147a0ffe8899baff1"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 99b509953b442d5efdd8f4c626a5bfeb0aca068c8f8ba0d71f4b871ec8a8d7f4
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
    "id": 134,
    "updated_at": "2016-11-09T11:18:48.304Z",
    "course_id": 195,
    "author_id": 592,
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
	-H "Authorization: Bearer 99b509953b442d5efdd8f4c626a5bfeb0aca068c8f8ba0d71f4b871ec8a8d7f4"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9b7419b3b3e3d41b798cba0f998f2bb6e2bbefaff5126276d628759e81aed3bb
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
      "id": 115,
      "updated_at": "2016-11-09T11:18:45.692Z",
      "course_id": 185,
      "author_id": 551,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 103",
      "position": 1
    },
    {
      "id": 116,
      "updated_at": "2016-11-09T11:18:45.719Z",
      "course_id": 185,
      "author_id": 552,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 104",
      "position": 2
    },
    {
      "id": 117,
      "updated_at": "2016-11-09T11:18:46.002Z",
      "course_id": 185,
      "author_id": 553,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-09T11:18:45.612Z",
      "questions_updated_at": "2016-11-09T11:18:45.612Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 105",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b7419b3b3e3d41b798cba0f998f2bb6e2bbefaff5126276d628759e81aed3bb"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1185ead030eacea74abeed42b65412c9b1f0a759bf5d431361aa264610e1cf4c
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
      "id": 118,
      "updated_at": "2016-11-09T11:18:46.299Z",
      "course_id": 187,
      "author_id": 560,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 106",
      "position": 1
    },
    {
      "id": 119,
      "updated_at": "2016-11-09T11:18:46.328Z",
      "course_id": 187,
      "author_id": 561,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 107",
      "position": 2
    },
    {
      "id": 120,
      "updated_at": "2016-11-09T11:18:46.358Z",
      "course_id": 187,
      "author_id": 562,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 108",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1185ead030eacea74abeed42b65412c9b1f0a759bf5d431361aa264610e1cf4c"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ceecc6cdffc0d47a49522a4d9e93e860ec55141810e99a72dd3609498ad5360c
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
	-H "Authorization: Bearer ceecc6cdffc0d47a49522a4d9e93e860ec55141810e99a72dd3609498ad5360c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/233
Content-Type: application/json
Authorization: Bearer 91273234a3d27670e1ef783c46e100dc9e7a2432d41f1860095937d3005cfb18
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/233" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91273234a3d27670e1ef783c46e100dc9e7a2432d41f1860095937d3005cfb18"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b478178eba2bf4cbdbf99108757dd1af17f0c2aaa9927fb922690d990568887e
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
    "creator_id": 680,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "discipline_id": 230,
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
    "chapters_updated_at": "2016-11-09T11:18:59.297Z",
    "updated_at": "2016-11-09T11:19:00.911Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 680,
        "chapter_id": 149,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.675Z",
        "created_at": "2016-11-09T11:19:00.675Z",
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
        "author_id": 680,
        "chapter_id": 150,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.755Z",
        "created_at": "2016-11-09T11:19:00.755Z",
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
        "author_id": 680,
        "chapter_id": 149,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.721Z",
        "created_at": "2016-11-09T11:19:00.721Z",
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
        "author_id": 680,
        "chapter_id": 150,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.800Z",
        "created_at": "2016-11-09T11:19:00.800Z",
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
        "author_id": 683,
        "chapter_id": 149,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.844Z",
        "created_at": "2016-11-09T11:19:00.844Z",
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
        "author_id": 684,
        "chapter_id": 150,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:00.890Z",
        "created_at": "2016-11-09T11:19:00.890Z",
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
        "id": 149,
        "updated_at": "2016-11-09T11:19:00.856Z",
        "course_id": 222,
        "author_id": 680,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T11:18:59.297Z",
        "questions_updated_at": "2016-11-09T11:18:59.297Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 134",
        "position": 1
      },
      {
        "id": 150,
        "updated_at": "2016-11-09T11:19:00.902Z",
        "course_id": 222,
        "author_id": 680,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T11:18:59.297Z",
        "questions_updated_at": "2016-11-09T11:18:59.297Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 135",
        "position": 2
      }
    ],
    "topic_id": 229,
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
	-H "Authorization: Bearer b478178eba2bf4cbdbf99108757dd1af17f0c2aaa9927fb922690d990568887e"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/218
Content-Type: application/json
Authorization: Bearer 9faef60ecdfb60d54341f84bd8dd4a8df0bdcdf9dfd3c756ea7d9a7ec7eb7f44
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
    "creator_id": 668,
    "id": 218,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 203,
    "additional_university_ids": [

    ],
    "discipline_id": 226,
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
    "updated_at": "2016-11-09T11:18:57.199Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 225,
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
curl "api.goskive.com/v2/courses/218" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9faef60ecdfb60d54341f84bd8dd4a8df0bdcdf9dfd3c756ea7d9a7ec7eb7f44"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f010624c26d1dcf21f326c9cdbaaa4253bae3aa1154bcfc071c134e57e85afc0
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
    "creator_id": 664,
    "id": 216,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 201,
    "additional_university_ids": [

    ],
    "discipline_id": 224,
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
    "updated_at": "2016-11-09T11:18:56.922Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 223,
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
	-H "Authorization: Bearer f010624c26d1dcf21f326c9cdbaaa4253bae3aa1154bcfc071c134e57e85afc0"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 09a8e084ed8af6e5237975f7357325563b5946512be3ec99e0e3d6b5a88178e7
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
      "id": 33,
      "user_id": 831,
      "feedbackable_id": 130,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:19:16.060Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 835,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:19:16.376Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 839,
      "feedbackable_id": 132,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:19:16.695Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 843,
      "feedbackable_id": 133,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:19:17.018Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 37,
      "user_id": 847,
      "feedbackable_id": 134,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T11:19:17.353Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09a8e084ed8af6e5237975f7357325563b5946512be3ec99e0e3d6b5a88178e7"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 63ec4a7e099f3dd46d9663719067505689f389fd2f3102d109dd3a4ec85c0dfe
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
      "id": 32,
      "user_id": 826,
      "feedbackable_id": 129,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T11:19:15.686Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63ec4a7e099f3dd46d9663719067505689f389fd2f3102d109dd3a4ec85c0dfe"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 0a54ebddd1151117ac613f670c89df918b41a663bcaa9e50ae799bbd2f6021d3
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
	-H "Authorization: Bearer 0a54ebddd1151117ac613f670c89df918b41a663bcaa9e50ae799bbd2f6021d3"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/3/metadata
Content-Type: application/json
Authorization: Bearer 6c04dfdfcaaca483613ea55d86442d422bb0679b8da596e241cf132f1e9b5f3c
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
    "id": 3,
    "uploader": {
      "id": 136,
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
      "created_at": "2016-11-09T11:18:09.448Z",
      "updated_at": "2016-11-09T11:18:09.448Z"
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
    "created_at": "2016-11-09T11:18:09.534Z",
    "updated_at": "2016-11-09T11:18:09.534Z",
    "course_id": 40,
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
curl "api.goskive.com/v2/files/3/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c04dfdfcaaca483613ea55d86442d422bb0679b8da596e241cf132f1e9b5f3c"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/7/feedbacks
Content-Type: application/json
Authorization: Bearer 7c71f4c4dc4bd23459f0a7008266107af45d2a869906cb3597c3b3e17fe773a9
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
      "id": 4,
      "user_id": 269,
      "feedbackable_id": 7,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:21.198Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 268,
      "feedbackable_id": 7,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:21.184Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/7/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c71f4c4dc4bd23459f0a7008266107af45d2a869906cb3597c3b3e17fe773a9"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer ea6746d5179977b1295f8c672058535adb7670c1cec553cce5241d65dff8e7af
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 406,
      "chapter_id": 82,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:30.947Z",
      "created_at": "2016-11-09T11:18:30.947Z",
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
      "author_id": 409,
      "chapter_id": 83,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:31.090Z",
      "created_at": "2016-11-09T11:18:31.090Z",
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
      "author_id": 412,
      "chapter_id": 84,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:31.231Z",
      "created_at": "2016-11-09T11:18:31.231Z",
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
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 415,
      "chapter_id": 85,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:31.378Z",
      "created_at": "2016-11-09T11:18:31.378Z",
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
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 418,
      "chapter_id": 86,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:31.521Z",
      "created_at": "2016-11-09T11:18:31.521Z",
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
	-H "Authorization: Bearer ea6746d5179977b1295f8c672058535adb7670c1cec553cce5241d65dff8e7af"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 6b62ba734aabfe22b6964f96c29d5d52f538324154c27c25c4a1447ef6f1c601
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 386,
      "chapter_id": 76,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:29.936Z",
      "created_at": "2016-11-09T11:18:29.936Z",
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
	-H "Authorization: Bearer 6b62ba734aabfe22b6964f96c29d5d52f538324154c27c25c4a1447ef6f1c601"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/15/republish
Content-Type: application/json
Authorization: Bearer cabb87f525d442d8383a0701515fbe0ea10eba23b4854167f63c37be84607a94
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/15/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cabb87f525d442d8383a0701515fbe0ea10eba23b4854167f63c37be84607a94"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/45/feedbacks
Content-Type: application/json
Authorization: Bearer 90dc1c4353c7cc967a3e38946152cde7c0f257bfa58f9ac4b916b84a9e548471
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
      "id": 16,
      "user_id": 322,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:24.873Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 321,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:24.861Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/45/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90dc1c4353c7cc967a3e38946152cde7c0f257bfa58f9ac4b916b84a9e548471"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer a5ac1433db89b67956d39c56f8138c75f77524415683be2908e3fdbee8d80b09
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 77,
      "chapter_id": 24,
      "position": 15,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:04.359Z",
      "created_at": "2016-11-09T11:18:04.229Z",
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
          "id": 48,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 49,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 68,
      "chapter_id": 21,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:03.455Z",
      "created_at": "2016-11-09T11:18:03.307Z",
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 71,
      "chapter_id": 22,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:03.761Z",
      "created_at": "2016-11-09T11:18:03.635Z",
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
    },
    {
      "id": 23,
      "obfuscated_id": "eUsQCUPDncM",
      "author_id": 74,
      "chapter_id": 23,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:04.059Z",
      "created_at": "2016-11-09T11:18:03.931Z",
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
          "id": 46,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 47,
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
      "author_id": 80,
      "chapter_id": 25,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:04.656Z",
      "created_at": "2016-11-09T11:18:04.533Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5ac1433db89b67956d39c56f8138c75f77524415683be2908e3fdbee8d80b09"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer f58fab4b24677e3654102d8747b465cf5bc79e46370bb89400f7d24597998097
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 48,
      "chapter_id": 15,
      "position": 6,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:01.404Z",
      "created_at": "2016-11-09T11:18:01.272Z",
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
          "id": 30,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 31,
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
	-H "Authorization: Bearer f58fab4b24677e3654102d8747b465cf5bc79e46370bb89400f7d24597998097"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/6/republish
Content-Type: application/json
Authorization: Bearer 0f33530135288566aee229f22e6846446ddf94f4e763c42121610f27247207f0
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/6/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f33530135288566aee229f22e6846446ddf94f4e763c42121610f27247207f0"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 902d6477be98fa111571aed72f539d4b3e92a0e6a79b880d7c8442de44c199ac
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":153,"published":false}}
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
    "creator_id": 501,
    "id": 146,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 153,
    "additional_university_ids": [

    ],
    "discipline_id": 154,
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
    "updated_at": "2016-11-09T11:18:41.340Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 153,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":153,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 902d6477be98fa111571aed72f539d4b3e92a0e6a79b880d7c8442de44c199ac"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1ae1b8154196479ff1073d60b4d01625cff0f0131026b1bf2f6f9a123ba81006
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
      "creator_id": 516,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "discipline_id": 167,
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
      "updated_at": "2016-11-09T11:18:42.698Z",
      "shortname": "fu-course-136",
      "topic_id": 166,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 516,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "discipline_id": 168,
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
      "updated_at": "2016-11-09T11:18:42.743Z",
      "shortname": "fu-course-137",
      "topic_id": 167,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 517,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "discipline_id": 169,
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
      "updated_at": "2016-11-09T11:18:42.796Z",
      "shortname": "fu-course-138",
      "topic_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 517,
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "discipline_id": 170,
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
      "chapters_updated_at": "2016-11-09T11:18:42.636Z",
      "updated_at": "2016-11-09T11:18:43.126Z",
      "shortname": "fu-course-139",
      "topic_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ae1b8154196479ff1073d60b4d01625cff0f0131026b1bf2f6f9a123ba81006"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 87fe6fe7a9473b071838edd77a7b554f3a2c06f736ab93b8ec46aafbd6265bb0
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
      "creator_id": 522,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-140",
      "html_url": "https://goskive.com/course/fu-course-140",
      "slug": "fu-course-140",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "discipline_id": 171,
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
      "updated_at": "2016-11-09T11:18:43.320Z",
      "shortname": "fu-course-140",
      "topic_id": 170,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 140",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 522,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "discipline_id": 172,
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
      "updated_at": "2016-11-09T11:18:43.362Z",
      "shortname": "fu-course-141",
      "topic_id": 171,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 523,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "discipline_id": 173,
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
      "updated_at": "2016-11-09T11:18:43.414Z",
      "shortname": "fu-course-142",
      "topic_id": 172,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 523,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-143",
      "html_url": "https://goskive.com/course/fu-course-143",
      "slug": "fu-course-143",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "discipline_id": 174,
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
      "updated_at": "2016-11-09T11:18:43.457Z",
      "shortname": "fu-course-143",
      "topic_id": 173,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87fe6fe7a9473b071838edd77a7b554f3a2c06f736ab93b8ec46aafbd6265bb0"
```
