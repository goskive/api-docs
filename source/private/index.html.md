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
DELETE /v2/chapters/42
Content-Type: application/json
Authorization: Bearer e52e538bee9bcfc2168a097899fef4408130302ed757de94206d2d19be8803c8
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/42" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e52e538bee9bcfc2168a097899fef4408130302ed757de94206d2d19be8803c8"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/47
Content-Type: application/json
Authorization: Bearer 06e04c96c26314b76e8d58aff1e61c5e8b1c98d8197fa8c7db56a6d2bf1a9312
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
    "id": 47,
    "updated_at": "2016-11-08T20:46:58.872Z",
    "course_id": 87,
    "author_id": 198,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-08T20:46:58.354Z",
    "questions_updated_at": "2016-11-08T20:46:58.354Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 201,
        "chapter_id": 47,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.820Z",
        "created_at": "2016-11-08T20:46:58.820Z",
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
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 202,
        "chapter_id": 47,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.855Z",
        "created_at": "2016-11-08T20:46:58.855Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 199,
        "chapter_id": 47,
        "position": 22,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.571Z",
        "created_at": "2016-11-08T20:46:58.460Z",
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
            "id": 43,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 44,
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
        "author_id": 200,
        "chapter_id": 47,
        "position": 23,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.754Z",
        "created_at": "2016-11-08T20:46:58.638Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06e04c96c26314b76e8d58aff1e61c5e8b1c98d8197fa8c7db56a6d2bf1a9312"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/50
Content-Type: application/json
Authorization: Bearer 5b98c06819f59e4782608e4070ba559846e8dbabeeb4b42ef09009131108f4f0
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
    "id": 50,
    "updated_at": "2016-11-08T20:46:59.414Z",
    "course_id": 90,
    "author_id": 210,
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
curl "api.goskive.com/v2/chapters/50" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b98c06819f59e4782608e4070ba559846e8dbabeeb4b42ef09009131108f4f0"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/44
Content-Type: application/json
Authorization: Bearer caf2be1dc1df8307b1c661bfdf8b14ea0238b21fa656f6bd452a76243543be8b
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
	-H "Authorization: Bearer caf2be1dc1df8307b1c661bfdf8b14ea0238b21fa656f6bd452a76243543be8b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 19c0965eb3093cbe393fb76bc7dc9b749ef37aea01422c20641caffe0d756bfd
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
      "id": 6,
      "author_id": 412,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:17.511Z",
      "status": "published",
      "subject_id": 137,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 414,
      "reply_to_id": 6,
      "created_at": "2016-11-08T20:47:17.591Z",
      "status": "published",
      "subject_id": 138,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 8,
      "author_id": 416,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:17.674Z",
      "status": "published",
      "subject_id": 139,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 418,
      "reply_to_id": 8,
      "created_at": "2016-11-08T20:47:17.755Z",
      "status": "published",
      "subject_id": 140,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 420,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:17.837Z",
      "status": "reported",
      "subject_id": 141,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 422,
      "reply_to_id": 10,
      "created_at": "2016-11-08T20:47:17.922Z",
      "status": "published",
      "subject_id": 142,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 424,
      "reply_to_id": 10,
      "created_at": "2016-11-08T20:47:18.004Z",
      "status": "published",
      "subject_id": 143,
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
	-H "Authorization: Bearer 19c0965eb3093cbe393fb76bc7dc9b749ef37aea01422c20641caffe0d756bfd"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c1c72104aaa5c053bebece83fbaf8cec5a400d2d2350bb26a030b2ec7f3d5f87
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
      "author_id": 472,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:20.067Z",
      "status": "published",
      "subject_id": 165,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 474,
      "reply_to_id": 34,
      "created_at": "2016-11-08T20:47:20.150Z",
      "status": "published",
      "subject_id": 166,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 476,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:20.232Z",
      "status": "published",
      "subject_id": 167,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 478,
      "reply_to_id": 36,
      "created_at": "2016-11-08T20:47:20.311Z",
      "status": "published",
      "subject_id": 168,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 480,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:20.394Z",
      "status": "reported",
      "subject_id": 169,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 482,
      "reply_to_id": 38,
      "created_at": "2016-11-08T20:47:20.475Z",
      "status": "published",
      "subject_id": 170,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 484,
      "reply_to_id": 38,
      "created_at": "2016-11-08T20:47:20.559Z",
      "status": "published",
      "subject_id": 171,
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
	-H "Authorization: Bearer c1c72104aaa5c053bebece83fbaf8cec5a400d2d2350bb26a030b2ec7f3d5f87"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 80d7a98c407b0f2bf83bd8658e88496771b71be3cfeee4b98ee6b3ce345d320f
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
      "author_id": 459,
      "reply_to_id": 27,
      "created_at": "2016-11-08T20:47:19.527Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 463,
      "reply_to_id": 29,
      "created_at": "2016-11-08T20:47:19.691Z",
      "status": "published",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 467,
      "reply_to_id": 31,
      "created_at": "2016-11-08T20:47:19.855Z",
      "status": "published",
      "subject_id": 163,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 469,
      "reply_to_id": 31,
      "created_at": "2016-11-08T20:47:19.936Z",
      "status": "published",
      "subject_id": 164,
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
	-H "Authorization: Bearer 80d7a98c407b0f2bf83bd8658e88496771b71be3cfeee4b98ee6b3ce345d320f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer b797ec9159913de46bf326810b6071dba67adaf75023f6fcc251b0788a91acca
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
      "id": 24,
      "author_id": 450,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:19.155Z",
      "status": "reported",
      "subject_id": 155,
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
	-H "Authorization: Bearer b797ec9159913de46bf326810b6071dba67adaf75023f6fcc251b0788a91acca"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/41/republish
Content-Type: application/json
Authorization: Bearer cbdfbfa7d1e2a697b99f5c3777a0152be568be95fb1d1295ca2555d59211dfdf
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/41/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbdfbfa7d1e2a697b99f5c3777a0152be568be95fb1d1295ca2555d59211dfdf"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/12/chapters
Content-Type: application/json
Authorization: Bearer 5b88b3a3008adbe2148e25492d0766ff6b55d74aa7b927244650394c62269d82
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
    "id": 22,
    "updated_at": "2016-11-08T20:46:44.272Z",
    "course_id": 12,
    "author_id": 54,
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
curl "api.goskive.com/v2/courses/12/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b88b3a3008adbe2148e25492d0766ff6b55d74aa7b927244650394c62269d82"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5a0d7937217bafd11638fb76dcf1837f51cc58b2e05ff0cc5207140c74fcadf9
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
    "id": 23,
    "updated_at": "2016-11-08T20:46:44.602Z",
    "course_id": 13,
    "author_id": 56,
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
	-H "Authorization: Bearer 5a0d7937217bafd11638fb76dcf1837f51cc58b2e05ff0cc5207140c74fcadf9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6d1ba92566c87d0ee84f62629d5bfa062ed6f7c19a566f1863b28194040dab80
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
      "id": 1,
      "updated_at": "2016-11-08T20:46:41.706Z",
      "course_id": 1,
      "author_id": 8,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 1",
      "position": 1
    },
    {
      "id": 2,
      "updated_at": "2016-11-08T20:46:41.734Z",
      "course_id": 1,
      "author_id": 9,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 2",
      "position": 2
    },
    {
      "id": 3,
      "updated_at": "2016-11-08T20:46:42.068Z",
      "course_id": 1,
      "author_id": 10,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-08T20:46:41.323Z",
      "questions_updated_at": "2016-11-08T20:46:41.323Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 3",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d1ba92566c87d0ee84f62629d5bfa062ed6f7c19a566f1863b28194040dab80"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 354207236b5406f08506e1c7398b4af310b69cb6a4118d70256fd0a5233edc06
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
      "id": 4,
      "updated_at": "2016-11-08T20:46:42.398Z",
      "course_id": 3,
      "author_id": 17,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 4",
      "position": 1
    },
    {
      "id": 5,
      "updated_at": "2016-11-08T20:46:42.422Z",
      "course_id": 3,
      "author_id": 18,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 5",
      "position": 2
    },
    {
      "id": 6,
      "updated_at": "2016-11-08T20:46:42.446Z",
      "course_id": 3,
      "author_id": 19,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 6",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 354207236b5406f08506e1c7398b4af310b69cb6a4118d70256fd0a5233edc06"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/251
Content-Type: application/json
Authorization: Bearer 9555606622231fbeeaf244d126b7a151046500b790c8a6cce87754a6f5a1f381
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/251" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9555606622231fbeeaf244d126b7a151046500b790c8a6cce87754a6f5a1f381"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer be373d06d4bdc95c72bb5ecde95601f1b13b5ff4737df1ca7fe7ce1b98a310e6
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
	-H "Authorization: Bearer be373d06d4bdc95c72bb5ecde95601f1b13b5ff4737df1ca7fe7ce1b98a310e6"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 2657a06ef82705106b751ad044df8e1326a3ad46d30f4e7df05cec01847093d3
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
    "creator_id": 772,
    "id": 249,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 234,
    "additional_university_ids": [

    ],
    "discipline_id": 262,
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
    "chapters_updated_at": "2016-11-08T20:47:44.036Z",
    "updated_at": "2016-11-08T20:47:45.606Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 772,
        "chapter_id": 146,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.381Z",
        "created_at": "2016-11-08T20:47:45.381Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 772,
        "chapter_id": 147,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.459Z",
        "created_at": "2016-11-08T20:47:45.459Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 772,
        "chapter_id": 146,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.427Z",
        "created_at": "2016-11-08T20:47:45.427Z",
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
        "author_id": 772,
        "chapter_id": 147,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.504Z",
        "created_at": "2016-11-08T20:47:45.504Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 775,
        "chapter_id": 146,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.547Z",
        "created_at": "2016-11-08T20:47:45.547Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 776,
        "chapter_id": 147,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:45.587Z",
        "created_at": "2016-11-08T20:47:45.587Z",
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
        "id": 146,
        "updated_at": "2016-11-08T20:47:45.558Z",
        "course_id": 249,
        "author_id": 772,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-08T20:47:44.036Z",
        "questions_updated_at": "2016-11-08T20:47:44.036Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 128",
        "position": 1
      },
      {
        "id": 147,
        "updated_at": "2016-11-08T20:47:45.598Z",
        "course_id": 249,
        "author_id": 772,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-08T20:47:44.036Z",
        "questions_updated_at": "2016-11-08T20:47:44.036Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 129",
        "position": 2
      }
    ],
    "topic_id": 261,
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
	-H "Authorization: Bearer 2657a06ef82705106b751ad044df8e1326a3ad46d30f4e7df05cec01847093d3"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/263
Content-Type: application/json
Authorization: Bearer 30c3a992f2e544ec974dae45b19b0dd903a4546f1ad93d7459491a346fdbba36
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
    "creator_id": 805,
    "id": 263,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 248,
    "additional_university_ids": [

    ],
    "discipline_id": 276,
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
    "updated_at": "2016-11-08T20:47:48.040Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 275,
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
curl "api.goskive.com/v2/courses/263" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30c3a992f2e544ec974dae45b19b0dd903a4546f1ad93d7459491a346fdbba36"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1545235cc9a035f54f6672290c5baf84dfe19ca246a5dbbb70b9d220904d618b
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
    "creator_id": 801,
    "id": 261,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 246,
    "additional_university_ids": [

    ],
    "discipline_id": 274,
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
    "updated_at": "2016-11-08T20:47:47.790Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 273,
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
	-H "Authorization: Bearer 1545235cc9a035f54f6672290c5baf84dfe19ca246a5dbbb70b9d220904d618b"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer ae11037135899fad5d99be5939afb471b7b439ba825b4f537feab85fd291b497
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
      "id": 23,
      "user_id": 321,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:07.367Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 325,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:07.660Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 329,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:07.956Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 333,
      "feedbackable_id": 41,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:08.256Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 337,
      "feedbackable_id": 42,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-08T20:47:08.560Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae11037135899fad5d99be5939afb471b7b439ba825b4f537feab85fd291b497"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 12ec5937fc97d5ffcbe4fefa7d424d22bbf446d6fac68f5337b0c668c042838c
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
      "id": 13,
      "user_id": 279,
      "feedbackable_id": 28,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-08T20:47:04.064Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12ec5937fc97d5ffcbe4fefa7d424d22bbf446d6fac68f5337b0c668c042838c"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer bf11033eed6332ce659fcf1bd17087937049fce7c67a796808cfe92b8ef7ad32
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
	-H "Authorization: Bearer bf11033eed6332ce659fcf1bd17087937049fce7c67a796808cfe92b8ef7ad32"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer ecf95736d65d3d2688e4beae2e2303ae2ea413752ee50220220b883757a7192a
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
    "id": 10,
    "uploader": {
      "id": 720,
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
      "created_at": "2016-11-08T20:47:37.092Z",
      "updated_at": "2016-11-08T20:47:37.092Z"
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
    "created_at": "2016-11-08T20:47:37.165Z",
    "updated_at": "2016-11-08T20:47:37.165Z",
    "course_id": 234,
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
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecf95736d65d3d2688e4beae2e2303ae2ea413752ee50220220b883757a7192a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/31/feedbacks
Content-Type: application/json
Authorization: Bearer 1af22f206234a2988eaa02c6173fe67ee3c0f12dce7efef48b05adba6bdf3f57
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
      "id": 35,
      "user_id": 527,
      "feedbackable_id": 31,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:22.902Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 526,
      "feedbackable_id": 31,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:22.891Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/31/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1af22f206234a2988eaa02c6173fe67ee3c0f12dce7efef48b05adba6bdf3f57"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 66b1bf3eda84c9c2ad76db213d6ca352a1ff7d97204c57557c93b43acdc395a4
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 639,
      "chapter_id": 115,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:32.614Z",
      "created_at": "2016-11-08T20:47:32.614Z",
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
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 642,
      "chapter_id": 116,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:32.749Z",
      "created_at": "2016-11-08T20:47:32.749Z",
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
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 645,
      "chapter_id": 117,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:32.887Z",
      "created_at": "2016-11-08T20:47:32.887Z",
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 648,
      "chapter_id": 118,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:33.020Z",
      "created_at": "2016-11-08T20:47:33.020Z",
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
      "author_id": 651,
      "chapter_id": 119,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:33.155Z",
      "created_at": "2016-11-08T20:47:33.155Z",
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
	-H "Authorization: Bearer 66b1bf3eda84c9c2ad76db213d6ca352a1ff7d97204c57557c93b43acdc395a4"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 273759d0c37d1f4212a56105ec961d262a9eeaa5f179cde03dbf147b78a50a34
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 667,
      "chapter_id": 124,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:33.887Z",
      "created_at": "2016-11-08T20:47:33.887Z",
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
	-H "Authorization: Bearer 273759d0c37d1f4212a56105ec961d262a9eeaa5f179cde03dbf147b78a50a34"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/59/republish
Content-Type: application/json
Authorization: Bearer 027d59a4cedd82fafe58214ecbd445984f7a88ed58541ce55a11aa457842d1c7
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/59/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 027d59a4cedd82fafe58214ecbd445984f7a88ed58541ce55a11aa457842d1c7"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/129/feedbacks
Content-Type: application/json
Authorization: Bearer 56b26b9c6115e6ef33be4d017b2ac8d344a0b171b2715fbe73c9abce2023d724
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
      "user_id": 963,
      "feedbackable_id": 129,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:48:04.674Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 962,
      "feedbackable_id": 129,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:48:04.662Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/129/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56b26b9c6115e6ef33be4d017b2ac8d344a0b171b2715fbe73c9abce2023d724"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 56a2804bf7c026687f2c905037258751c9603694e2aaea7f72ee6fa8e91577c1
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
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 912,
      "chapter_id": 174,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:58.389Z",
      "created_at": "2016-11-08T20:47:58.272Z",
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
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 915,
      "chapter_id": 175,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:58.674Z",
      "created_at": "2016-11-08T20:47:58.554Z",
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
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 918,
      "chapter_id": 176,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:58.960Z",
      "created_at": "2016-11-08T20:47:58.837Z",
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
          "id": 232,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 233,
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
      "author_id": 921,
      "chapter_id": 177,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:59.247Z",
      "created_at": "2016-11-08T20:47:59.124Z",
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
          "id": 234,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 235,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 924,
      "chapter_id": 178,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:59.526Z",
      "created_at": "2016-11-08T20:47:59.410Z",
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
          "id": 236,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 237,
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
	-H "Authorization: Bearer 56a2804bf7c026687f2c905037258751c9603694e2aaea7f72ee6fa8e91577c1"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 80d10da5f88a2f5bc4eb2648526cce587df6b4a72727922d898311709c3f7d20
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
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 908,
      "chapter_id": 173,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:58.056Z",
      "created_at": "2016-11-08T20:47:57.932Z",
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
          "id": 226,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 227,
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
	-H "Authorization: Bearer 80d10da5f88a2f5bc4eb2648526cce587df6b4a72727922d898311709c3f7d20"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/123/republish
Content-Type: application/json
Authorization: Bearer 13d138841de1f3fa9a10e7b26bd205c3a10a0cb207beb2fefa5fe30c83b778df
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/123/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13d138841de1f3fa9a10e7b26bd205c3a10a0cb207beb2fefa5fe30c83b778df"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 572fac72484cfde4fb8a270e40d4cdba3eb268d7de0fdc758e5a4df197b35d23
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":18,"published":false}}
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
    "creator_id": 61,
    "id": 16,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 16,
    "additional_university_ids": [

    ],
    "discipline_id": 19,
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
    "updated_at": "2016-11-08T20:46:45.209Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 18,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":18,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 572fac72484cfde4fb8a270e40d4cdba3eb268d7de0fdc758e5a4df197b35d23"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 28465b70c4a24dc1db50daac2d8f4cce6af3a678dbf02f4a636f8cd49f5f9ab1
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
      "creator_id": 69,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-5",
      "html_url": "https://goskive.com/course/fu-course-5",
      "slug": "fu-course-5",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "discipline_id": 27,
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
      "updated_at": "2016-11-08T20:46:46.419Z",
      "shortname": "fu-course-5",
      "topic_id": 26,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 69,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-6",
      "html_url": "https://goskive.com/course/fu-course-6",
      "slug": "fu-course-6",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "discipline_id": 28,
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
      "updated_at": "2016-11-08T20:46:46.459Z",
      "shortname": "fu-course-6",
      "topic_id": 27,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 70,
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "discipline_id": 29,
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
      "updated_at": "2016-11-08T20:46:46.506Z",
      "shortname": "fu-course-7",
      "topic_id": 28,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 70,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "discipline_id": 30,
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
      "chapters_updated_at": "2016-11-08T20:46:46.359Z",
      "updated_at": "2016-11-08T20:46:46.800Z",
      "shortname": "fu-course-8",
      "topic_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 8",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28465b70c4a24dc1db50daac2d8f4cce6af3a678dbf02f4a636f8cd49f5f9ab1"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 080ee0fbe336824ec1cd44dc665dae4d3ddab765bcdc097c29cc4ad2db6c52f9
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
      "creator_id": 76,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-9",
      "html_url": "https://goskive.com/course/fu-course-9",
      "slug": "fu-course-9",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "discipline_id": 31,
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
      "updated_at": "2016-11-08T20:46:47.003Z",
      "shortname": "fu-course-9",
      "topic_id": 30,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 9",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 76,
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-10",
      "html_url": "https://goskive.com/course/fu-course-10",
      "slug": "fu-course-10",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "discipline_id": 32,
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
      "updated_at": "2016-11-08T20:46:47.041Z",
      "shortname": "fu-course-10",
      "topic_id": 31,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 10",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 77,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "discipline_id": 33,
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
      "updated_at": "2016-11-08T20:46:47.086Z",
      "shortname": "fu-course-11",
      "topic_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 77,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "discipline_id": 34,
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
      "updated_at": "2016-11-08T20:46:47.122Z",
      "shortname": "fu-course-12",
      "topic_id": 33,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 080ee0fbe336824ec1cd44dc665dae4d3ddab765bcdc097c29cc4ad2db6c52f9"
```
