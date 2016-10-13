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
Authorization: Bearer 465121bb8bc1401ceb1c1c1dd5660ddd8b23815ea865872a7ef0c4c4583630b9
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
	-H "Authorization: Bearer 465121bb8bc1401ceb1c1c1dd5660ddd8b23815ea865872a7ef0c4c4583630b9"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/47
Content-Type: application/json
Authorization: Bearer 5ddf61ab3017e8f2f17058aae6ee68cdf7cd3cd99deb8180fd9d2254a8678e14
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
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T14:00:12.526Z",
    "course_id": 141,
    "author_id": 343,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-13T14:00:11.873Z",
    "questions_updated_at": "2016-10-13T14:00:11.873Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 346,
        "chapter_id": 47,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:12.464Z",
        "created_at": "2016-10-13T14:00:12.464Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 347,
        "chapter_id": 47,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:12.506Z",
        "created_at": "2016-10-13T14:00:12.506Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 344,
        "chapter_id": 47,
        "position": 43,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:12.147Z",
        "created_at": "2016-10-13T14:00:12.008Z",
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
            "id": 85,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 86,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 345,
        "chapter_id": 47,
        "position": 44,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:12.382Z",
        "created_at": "2016-10-13T14:00:12.234Z",
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
            "id": 87,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 88,
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
curl "api.goskive.com/v2/chapters/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ddf61ab3017e8f2f17058aae6ee68cdf7cd3cd99deb8180fd9d2254a8678e14"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/44
Content-Type: application/json
Authorization: Bearer 9bb3fc0d485b45cd5171a0db3e28e7aa4d321aae23dd0d234e4843ef93d946cc
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
    "id": 44,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T14:00:10.967Z",
    "course_id": 138,
    "author_id": 331,
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
curl "api.goskive.com/v2/chapters/44" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bb3fc0d485b45cd5171a0db3e28e7aa4d321aae23dd0d234e4843ef93d946cc"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer a55760f6a3fdbd52c8fa793ef1e952e74457fcfdd696d3323f8bbc14a3851135
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a55760f6a3fdbd52c8fa793ef1e952e74457fcfdd696d3323f8bbc14a3851135"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d2228a674b359a71a5fab12dc305cd21b6d19c48b884d815438dfb600441f43d
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
      "id": 13,
      "author_id": 118,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:55.726Z",
      "status": "published",
      "subject_id": 40,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 120,
      "reply_to_id": 13,
      "created_at": "2016-10-13T13:59:55.807Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 122,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:55.911Z",
      "status": "published",
      "subject_id": 42,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 124,
      "reply_to_id": 15,
      "created_at": "2016-10-13T13:59:56.001Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 126,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:56.087Z",
      "status": "reported",
      "subject_id": 44,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 128,
      "reply_to_id": 17,
      "created_at": "2016-10-13T13:59:56.171Z",
      "status": "published",
      "subject_id": 45,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 130,
      "reply_to_id": 17,
      "created_at": "2016-10-13T13:59:56.266Z",
      "status": "published",
      "subject_id": 46,
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
	-H "Authorization: Bearer d2228a674b359a71a5fab12dc305cd21b6d19c48b884d815438dfb600441f43d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 64103bfda995d79b8c8bf290bf9f16256d251f8a92d91e9d79aa171bd68968d5
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
      "id": 27,
      "author_id": 148,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:57.100Z",
      "status": "published",
      "subject_id": 54,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 150,
      "reply_to_id": 27,
      "created_at": "2016-10-13T13:59:57.200Z",
      "status": "published",
      "subject_id": 55,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 152,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:57.294Z",
      "status": "published",
      "subject_id": 56,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 154,
      "reply_to_id": 29,
      "created_at": "2016-10-13T13:59:57.390Z",
      "status": "published",
      "subject_id": 57,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 156,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:57.482Z",
      "status": "reported",
      "subject_id": 58,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 158,
      "reply_to_id": 31,
      "created_at": "2016-10-13T13:59:57.571Z",
      "status": "published",
      "subject_id": 59,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 160,
      "reply_to_id": 31,
      "created_at": "2016-10-13T13:59:57.658Z",
      "status": "published",
      "subject_id": 60,
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
	-H "Authorization: Bearer 64103bfda995d79b8c8bf290bf9f16256d251f8a92d91e9d79aa171bd68968d5"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 77a37932559e69903ecefbfcd3b10f1c1a917023b87ed4c2a2eab32ba6974f62
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
      "id": 21,
      "author_id": 135,
      "reply_to_id": 20,
      "created_at": "2016-10-13T13:59:56.506Z",
      "status": "published",
      "subject_id": 48,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 139,
      "reply_to_id": 22,
      "created_at": "2016-10-13T13:59:56.685Z",
      "status": "published",
      "subject_id": 50,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 143,
      "reply_to_id": 24,
      "created_at": "2016-10-13T13:59:56.863Z",
      "status": "published",
      "subject_id": 52,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 145,
      "reply_to_id": 24,
      "created_at": "2016-10-13T13:59:56.953Z",
      "status": "published",
      "subject_id": 53,
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
	-H "Authorization: Bearer 77a37932559e69903ecefbfcd3b10f1c1a917023b87ed4c2a2eab32ba6974f62"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 8cc3930bf3db57eef0e23cb65f0b60894631bd6a6627a598064444e3513ce19a
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
      "id": 10,
      "author_id": 111,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:59:55.430Z",
      "status": "reported",
      "subject_id": 37,
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
	-H "Authorization: Bearer 8cc3930bf3db57eef0e23cb65f0b60894631bd6a6627a598064444e3513ce19a"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/2/republish
Content-Type: application/json
Authorization: Bearer 590c4903e4c4aa495c60084dffe909446f5b198b2d7fd547fd8ad1b232302950
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/2/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 590c4903e4c4aa495c60084dffe909446f5b198b2d7fd547fd8ad1b232302950"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/148/chapters
Content-Type: application/json
Authorization: Bearer 3422fd2d55558f580f9972b329ccfeb52708cfd673f6ab9bd0efb41d4b1a0ff8
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
    "id": 48,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T14:00:14.160Z",
    "course_id": 148,
    "author_id": 368,
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
curl "api.goskive.com/v2/courses/148/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3422fd2d55558f580f9972b329ccfeb52708cfd673f6ab9bd0efb41d4b1a0ff8"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7758ecbda6b68f8b91a51f9432275b647ad3e6843282d81c658208a0e5201e3a
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
    "id": 49,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T14:00:14.292Z",
    "course_id": 149,
    "author_id": 370,
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
	-H "Authorization: Bearer 7758ecbda6b68f8b91a51f9432275b647ad3e6843282d81c658208a0e5201e3a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 20911b9d2c26f84d53abe568fb4189a7f7c5c74713c99d09a1eebc18ee81665e
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
      "id": 60,
      "title": "Clever Chapter Title 45",
      "position": 1,
      "updated_at": "2016-10-13T14:00:15.792Z",
      "course_id": 157,
      "author_id": 397,
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
      "id": 61,
      "title": "Clever Chapter Title 46",
      "position": 2,
      "updated_at": "2016-10-13T14:00:15.819Z",
      "course_id": 157,
      "author_id": 398,
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
      "id": 62,
      "title": "Clever Chapter Title 47",
      "position": 3,
      "updated_at": "2016-10-13T14:00:16.123Z",
      "course_id": 157,
      "author_id": 399,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-13T14:00:15.715Z",
      "questions_updated_at": "2016-10-13T14:00:15.715Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20911b9d2c26f84d53abe568fb4189a7f7c5c74713c99d09a1eebc18ee81665e"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 78b0620fe1c9f1a1f07e491de67034e5e2fe4dd7bb6577d05f02a5218c08a29f
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
      "id": 63,
      "title": "Clever Chapter Title 48",
      "position": 1,
      "updated_at": "2016-10-13T14:00:16.278Z",
      "course_id": 158,
      "author_id": 404,
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
      "id": 64,
      "title": "Clever Chapter Title 49",
      "position": 2,
      "updated_at": "2016-10-13T14:00:16.305Z",
      "course_id": 158,
      "author_id": 405,
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
      "id": 65,
      "title": "Clever Chapter Title 50",
      "position": 3,
      "updated_at": "2016-10-13T14:00:16.332Z",
      "course_id": 158,
      "author_id": 406,
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
	-H "Authorization: Bearer 78b0620fe1c9f1a1f07e491de67034e5e2fe4dd7bb6577d05f02a5218c08a29f"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/9
Content-Type: application/json
Authorization: Bearer 247f89e4e934877fae82e988f4c6333b4e843cea936d8f484ec4fa83cb307561
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 247f89e4e934877fae82e988f4c6333b4e843cea936d8f484ec4fa83cb307561"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 573a03fd8c9394e6aaf28752dd5903a09c0f7809e0ec43009cea6136cb1eab04
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
	-H "Authorization: Bearer 573a03fd8c9394e6aaf28752dd5903a09c0f7809e0ec43009cea6136cb1eab04"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4c23769111035b3a099c289928baec5e630c2222b6b77b6bd820ea2a96dcb84e
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
    "creator_id": 59,
    "id": 21,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 21,
    "additional_university_ids": [

    ],
    "topic_id": 24,
    "discipline_id": 24,
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
    "chapters_updated_at": "2016-10-13T13:59:50.504Z",
    "updated_at": "2016-10-13T13:59:52.058Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 11,
        "title": "Clever Chapter Title 11",
        "position": 1,
        "updated_at": "2016-10-13T13:59:52.007Z",
        "course_id": 21,
        "author_id": 59,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T13:59:50.504Z",
        "questions_updated_at": "2016-10-13T13:59:50.504Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 12,
        "title": "Clever Chapter Title 12",
        "position": 2,
        "updated_at": "2016-10-13T13:59:52.050Z",
        "course_id": 21,
        "author_id": 59,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T13:59:50.504Z",
        "questions_updated_at": "2016-10-13T13:59:50.504Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 59,
        "chapter_id": 11,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:51.836Z",
        "created_at": "2016-10-13T13:59:51.836Z",
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
        "author_id": 59,
        "chapter_id": 12,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:51.910Z",
        "created_at": "2016-10-13T13:59:51.910Z",
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
        "author_id": 59,
        "chapter_id": 11,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:51.878Z",
        "created_at": "2016-10-13T13:59:51.878Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 59,
        "chapter_id": 12,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:51.954Z",
        "created_at": "2016-10-13T13:59:51.954Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 62,
        "chapter_id": 11,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:51.996Z",
        "created_at": "2016-10-13T13:59:51.996Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 63,
        "chapter_id": 12,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:52.038Z",
        "created_at": "2016-10-13T13:59:52.038Z",
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
	-H "Authorization: Bearer 4c23769111035b3a099c289928baec5e630c2222b6b77b6bd820ea2a96dcb84e"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/8
Content-Type: application/json
Authorization: Bearer ca23c1bafa96dc48fcb1bf5aa10490cd9b75aabe449b6fc957872b9b10fc49ba
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
    "creator_id": 20,
    "id": 8,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 8,
    "additional_university_ids": [

    ],
    "topic_id": 11,
    "discipline_id": 11,
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
    "updated_at": "2016-10-13T13:59:44.018Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/8" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca23c1bafa96dc48fcb1bf5aa10490cd9b75aabe449b6fc957872b9b10fc49ba"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 051797d4ce66f35ca555183e53df3b96b78c858a747e1fbbf68724c9209590fe
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
    "creator_id": 17,
    "id": 6,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 6,
    "additional_university_ids": [

    ],
    "topic_id": 9,
    "discipline_id": 9,
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
    "updated_at": "2016-10-13T13:59:43.710Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 051797d4ce66f35ca555183e53df3b96b78c858a747e1fbbf68724c9209590fe"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 70f7e839027ce4d517a51dba3d7522ca06215c2c53a9f978715ffaa39e92fc2e
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
      "id": 27,
      "user_id": 825,
      "feedbackable_id": 113,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:53.688Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 829,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:54.009Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 833,
      "feedbackable_id": 115,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:54.319Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 837,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:54.628Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 841,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T14:00:54.944Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70f7e839027ce4d517a51dba3d7522ca06215c2c53a9f978715ffaa39e92fc2e"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 886f51799eb3b5c659082a10d1ad61d421047e00c7cece3ab698a6c44af889ef
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
      "id": 36,
      "user_id": 862,
      "feedbackable_id": 122,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T14:00:56.543Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 886f51799eb3b5c659082a10d1ad61d421047e00c7cece3ab698a6c44af889ef"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Authorization: Bearer ece9f273d50581795f951cec1e6505322a67f43c3343ed1adfbf12d4d8096607
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
	-H "Authorization: Bearer ece9f273d50581795f951cec1e6505322a67f43c3343ed1adfbf12d4d8096607" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/33/feedbacks
Content-Type: application/json
Authorization: Bearer 3be9aa6be3e8e25f487d147ce74863f8c539aa0d25110112500b002525cb4893
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
      "user_id": 222,
      "feedbackable_id": 33,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:01.378Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 221,
      "feedbackable_id": 33,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:01.365Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3be9aa6be3e8e25f487d147ce74863f8c539aa0d25110112500b002525cb4893"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer fc31771c10a29d94b425dbba4558f79ba336560f4a11bed45419826e292a7e9c
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
      "author_id": 580,
      "chapter_id": 117,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:35.547Z",
      "created_at": "2016-10-13T14:00:35.547Z",
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
      "author_id": 583,
      "chapter_id": 118,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:35.684Z",
      "created_at": "2016-10-13T14:00:35.684Z",
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
      "author_id": 586,
      "chapter_id": 119,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:35.821Z",
      "created_at": "2016-10-13T14:00:35.821Z",
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
      "author_id": 589,
      "chapter_id": 120,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:35.962Z",
      "created_at": "2016-10-13T14:00:35.962Z",
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
      "author_id": 592,
      "chapter_id": 121,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:36.107Z",
      "created_at": "2016-10-13T14:00:36.107Z",
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
	-H "Authorization: Bearer fc31771c10a29d94b425dbba4558f79ba336560f4a11bed45419826e292a7e9c"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 792c3125921b00e1ac33d42fefc2fe3e49b9f0165a6aeacb0230532d42c60010
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 624,
      "chapter_id": 131,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:37.602Z",
      "created_at": "2016-10-13T14:00:37.602Z",
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
	-H "Authorization: Bearer 792c3125921b00e1ac33d42fefc2fe3e49b9f0165a6aeacb0230532d42c60010"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/51/republish
Content-Type: application/json
Authorization: Bearer e962266f189cb4f5b41a11d0b6d8fe06aae07a2d6435661bea5c0416c2acca09
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e962266f189cb4f5b41a11d0b6d8fe06aae07a2d6435661bea5c0416c2acca09"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/85/feedbacks
Content-Type: application/json
Authorization: Bearer 67be153b6908270c042be9bdf76dc2e417b2bc2520cd2140108b0be1bda9b67c
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
      "id": 15,
      "user_id": 548,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:33.670Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 547,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:33.658Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/85/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67be153b6908270c042be9bdf76dc2e417b2bc2520cd2140108b0be1bda9b67c"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 4e4f6cc1d8fd4f97d63df535fa2f2c4f4bcee24f58203886a0b86208e8cfe2f5
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
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 490,
      "chapter_id": 93,
      "position": 62,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:25.608Z",
      "created_at": "2016-10-13T14:00:25.439Z",
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
          "id": 137,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 138,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 481,
      "chapter_id": 90,
      "position": 59,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:24.550Z",
      "created_at": "2016-10-13T14:00:24.390Z",
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
          "id": 131,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 132,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 484,
      "chapter_id": 91,
      "position": 60,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:24.906Z",
      "created_at": "2016-10-13T14:00:24.742Z",
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
          "id": 133,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 134,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 487,
      "chapter_id": 92,
      "position": 61,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:25.254Z",
      "created_at": "2016-10-13T14:00:25.090Z",
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
          "id": 135,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 136,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 493,
      "chapter_id": 94,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:25.950Z",
      "created_at": "2016-10-13T14:00:25.795Z",
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
          "id": 139,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 140,
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
	-H "Authorization: Bearer 4e4f6cc1d8fd4f97d63df535fa2f2c4f4bcee24f58203886a0b86208e8cfe2f5"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c320e3fd82249e8bd7de53b5668468ff5fb851c588811103615b820aed2b78c1
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
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 461,
      "chapter_id": 84,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:22.331Z",
      "created_at": "2016-10-13T14:00:22.179Z",
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
          "id": 119,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 120,
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
	-H "Authorization: Bearer c320e3fd82249e8bd7de53b5668468ff5fb851c588811103615b820aed2b78c1"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/53/republish
Content-Type: application/json
Authorization: Bearer d42aeb135b22182769ec08b10b935c3aaa3d5e404890313356a926390b699312
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d42aeb135b22182769ec08b10b935c3aaa3d5e404890313356a926390b699312"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ecac9408d52cd236f9094ded3b24ea1db1e6c64560cc15270f8d5ddf1b0ba19b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":129,"published":false}}
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
    "creator_id": 288,
    "id": 124,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 129,
    "discipline_id": 129,
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
    "updated_at": "2016-10-13T14:00:06.623Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":129,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecac9408d52cd236f9094ded3b24ea1db1e6c64560cc15270f8d5ddf1b0ba19b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 943d901ba9e5aa8847353967fade9c09b4e3e17b755c170c3911c858e9d95b7d
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
      "creator_id": 252,
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-69",
      "html_url": "https://goskive.com/course/fu-course-69",
      "slug": "fu-course-69",
      "university_id": 90,
      "additional_university_ids": [

      ],
      "topic_id": 99,
      "discipline_id": 99,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T14:00:03.109Z",
      "shortname": "fu-course-69"
    },
    {
      "creator_id": 252,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-70",
      "html_url": "https://goskive.com/course/fu-course-70",
      "slug": "fu-course-70",
      "university_id": 90,
      "additional_university_ids": [

      ],
      "topic_id": 100,
      "discipline_id": 100,
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
      "updated_at": "2016-10-13T14:00:03.153Z",
      "shortname": "fu-course-70"
    },
    {
      "creator_id": 253,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-71",
      "html_url": "https://goskive.com/course/fu-course-71",
      "slug": "fu-course-71",
      "university_id": 90,
      "additional_university_ids": [

      ],
      "topic_id": 101,
      "discipline_id": 101,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T14:00:03.205Z",
      "shortname": "fu-course-71"
    },
    {
      "creator_id": 253,
      "id": 97,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-72",
      "html_url": "https://goskive.com/course/fu-course-72",
      "slug": "fu-course-72",
      "university_id": 90,
      "additional_university_ids": [

      ],
      "topic_id": 102,
      "discipline_id": 102,
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
      "chapters_updated_at": "2016-10-13T14:00:03.532Z",
      "updated_at": "2016-10-13T14:00:03.540Z",
      "shortname": "fu-course-72"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 943d901ba9e5aa8847353967fade9c09b4e3e17b755c170c3911c858e9d95b7d"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fdb786a6cf0c89da23dd9db9d0189c9c0f1aaeb9703db28c0eda331fd39c3e2e
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
      "creator_id": 259,
      "id": 98,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-73",
      "html_url": "https://goskive.com/course/fu-course-73",
      "slug": "fu-course-73",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 103,
      "discipline_id": 103,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T14:00:03.756Z",
      "shortname": "fu-course-73"
    },
    {
      "creator_id": 259,
      "id": 99,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-74",
      "html_url": "https://goskive.com/course/fu-course-74",
      "slug": "fu-course-74",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 104,
      "discipline_id": 104,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-13T14:00:03.799Z",
      "shortname": "fu-course-74"
    },
    {
      "creator_id": 260,
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-75",
      "html_url": "https://goskive.com/course/fu-course-75",
      "slug": "fu-course-75",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 105,
      "discipline_id": 105,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 75",
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
      "updated_at": "2016-10-13T14:00:03.850Z",
      "shortname": "fu-course-75"
    },
    {
      "creator_id": 260,
      "id": 101,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-76",
      "html_url": "https://goskive.com/course/fu-course-76",
      "slug": "fu-course-76",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 106,
      "discipline_id": 106,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 76",
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
      "updated_at": "2016-10-13T14:00:03.891Z",
      "shortname": "fu-course-76"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdb786a6cf0c89da23dd9db9d0189c9c0f1aaeb9703db28c0eda331fd39c3e2e"
```
