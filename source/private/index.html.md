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
DELETE /v2/chapters/6
Content-Type: application/json
Authorization: Bearer 93637accdb21e6e1d5fd1cec49c7e84ca5c472b9ae947950aac838ac530cc4ff
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93637accdb21e6e1d5fd1cec49c7e84ca5c472b9ae947950aac838ac530cc4ff"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/1
Content-Type: application/json
Authorization: Bearer 2df21aaa0e1cc85250db3a5eefe370f770492fdf10f5ebbae80cb525f29e7b94
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
    "id": 1,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T08:59:25.699Z",
    "course_id": 1,
    "author_id": 2,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-19T08:59:24.268Z",
    "questions_updated_at": "2016-10-19T08:59:24.268Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 5,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:25.642Z",
        "created_at": "2016-10-19T08:59:25.642Z",
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
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 6,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:25.682Z",
        "created_at": "2016-10-19T08:59:25.682Z",
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
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 3,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:25.372Z",
        "created_at": "2016-10-19T08:59:25.257Z",
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
            "id": 1,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 2,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 4,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:25.562Z",
        "created_at": "2016-10-19T08:59:25.445Z",
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
            "id": 3,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 4,
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
curl "api.goskive.com/v2/chapters/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2df21aaa0e1cc85250db3a5eefe370f770492fdf10f5ebbae80cb525f29e7b94"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 57d20e7e3099ac6bf00293708f4be0d10233aaba6f2d662e712d58bc8b139115
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
    "id": 7,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T08:59:27.703Z",
    "course_id": 7,
    "author_id": 28,
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
curl "api.goskive.com/v2/chapters/7" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57d20e7e3099ac6bf00293708f4be0d10233aaba6f2d662e712d58bc8b139115"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer ceddbc1c6532d248640ca38b3cdb535d0a85b5d6a130c8e01f659e56d82b8f40
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceddbc1c6532d248640ca38b3cdb535d0a85b5d6a130c8e01f659e56d82b8f40"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 8704e257d85c93d64c147dd0e3210f0e545bb0f4b3610bbbb86bbacd97665bc3
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
      "id": 10,
      "author_id": 676,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:24.075Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 678,
      "reply_to_id": 10,
      "created_at": "2016-10-19T09:00:24.165Z",
      "status": "published",
      "subject_id": 216,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 680,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:24.257Z",
      "status": "published",
      "subject_id": 217,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 682,
      "reply_to_id": 12,
      "created_at": "2016-10-19T09:00:24.347Z",
      "status": "published",
      "subject_id": 218,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 684,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:24.435Z",
      "status": "reported",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 686,
      "reply_to_id": 14,
      "created_at": "2016-10-19T09:00:24.521Z",
      "status": "published",
      "subject_id": 220,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 688,
      "reply_to_id": 14,
      "created_at": "2016-10-19T09:00:24.609Z",
      "status": "published",
      "subject_id": 221,
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
	-H "Authorization: Bearer 8704e257d85c93d64c147dd0e3210f0e545bb0f4b3610bbbb86bbacd97665bc3"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c93eceb0db922c1fd1ee84acb07900c5c8863dc7eaed8deccdc406c6cbeb7c26
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
      "id": 38,
      "author_id": 736,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:26.932Z",
      "status": "published",
      "subject_id": 243,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 738,
      "reply_to_id": 38,
      "created_at": "2016-10-19T09:00:27.025Z",
      "status": "published",
      "subject_id": 244,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 740,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:27.117Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 742,
      "reply_to_id": 40,
      "created_at": "2016-10-19T09:00:27.210Z",
      "status": "published",
      "subject_id": 246,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 744,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:27.305Z",
      "status": "reported",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 746,
      "reply_to_id": 42,
      "created_at": "2016-10-19T09:00:27.401Z",
      "status": "published",
      "subject_id": 248,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 748,
      "reply_to_id": 42,
      "created_at": "2016-10-19T09:00:27.500Z",
      "status": "published",
      "subject_id": 249,
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
	-H "Authorization: Bearer c93eceb0db922c1fd1ee84acb07900c5c8863dc7eaed8deccdc406c6cbeb7c26"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer a8a332995f9373f1322cc99d2f66bb54e9ff7a6f4f3f84534b5a10fd4e06fb4d
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
      "id": 25,
      "author_id": 708,
      "reply_to_id": 24,
      "created_at": "2016-10-19T09:00:25.579Z",
      "status": "published",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 712,
      "reply_to_id": 26,
      "created_at": "2016-10-19T09:00:25.771Z",
      "status": "published",
      "subject_id": 232,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 716,
      "reply_to_id": 28,
      "created_at": "2016-10-19T09:00:25.955Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 718,
      "reply_to_id": 28,
      "created_at": "2016-10-19T09:00:26.049Z",
      "status": "published",
      "subject_id": 235,
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
	-H "Authorization: Bearer a8a332995f9373f1322cc99d2f66bb54e9ff7a6f4f3f84534b5a10fd4e06fb4d"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer e8d3786b90e6fb4eea601505be0ed9fa38939b17664093d9c0a78fe953156497
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
      "id": 21,
      "author_id": 699,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:25.141Z",
      "status": "reported",
      "subject_id": 226,
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
	-H "Authorization: Bearer e8d3786b90e6fb4eea601505be0ed9fa38939b17664093d9c0a78fe953156497"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/45/republish
Content-Type: application/json
Authorization: Bearer 497456f617afc485f9c00233d149c6d6d24c7de9088bbd74da4d51fa67d81950
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/45/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 497456f617afc485f9c00233d149c6d6d24c7de9088bbd74da4d51fa67d81950"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/262/chapters
Content-Type: application/json
Authorization: Bearer b6a5fc86f1c2d403fd4e73b0d77e6bfc4b46ef36cd3921bb809d2221e4c2952b
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
    "id": 151,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T09:00:31.085Z",
    "course_id": 262,
    "author_id": 790,
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
curl "api.goskive.com/v2/courses/262/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6a5fc86f1c2d403fd4e73b0d77e6bfc4b46ef36cd3921bb809d2221e4c2952b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4b525fc335d9b56e6adde6b5f104239090ca7c389914bb7b2e91e4dbbd7f819f
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
    "id": 152,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T09:00:31.368Z",
    "course_id": 264,
    "author_id": 794,
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
	-H "Authorization: Bearer 4b525fc335d9b56e6adde6b5f104239090ca7c389914bb7b2e91e4dbbd7f819f"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer efbd9f3635475f057264806506c69bc0aa9f9b958b39c1212785af05f500fb9a
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
      "id": 166,
      "title": "Clever Chapter Title 142",
      "position": 1,
      "updated_at": "2016-10-19T09:00:33.046Z",
      "course_id": 272,
      "author_id": 823,
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
      "id": 167,
      "title": "Clever Chapter Title 143",
      "position": 2,
      "updated_at": "2016-10-19T09:00:33.070Z",
      "course_id": 272,
      "author_id": 824,
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
      "id": 168,
      "title": "Clever Chapter Title 144",
      "position": 3,
      "updated_at": "2016-10-19T09:00:33.320Z",
      "course_id": 272,
      "author_id": 825,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-19T09:00:32.970Z",
      "questions_updated_at": "2016-10-19T09:00:32.970Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer efbd9f3635475f057264806506c69bc0aa9f9b958b39c1212785af05f500fb9a"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e6dd172a5fb7866f2e36e8994bd7206624681607ed04e65d410a487d99a51eed
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
      "id": 169,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-19T09:00:33.472Z",
      "course_id": 273,
      "author_id": 830,
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
      "id": 170,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-19T09:00:33.497Z",
      "course_id": 273,
      "author_id": 831,
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
      "id": 171,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-19T09:00:33.522Z",
      "course_id": 273,
      "author_id": 832,
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
	-H "Authorization: Bearer e6dd172a5fb7866f2e36e8994bd7206624681607ed04e65d410a487d99a51eed"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/73
Content-Type: application/json
Authorization: Bearer f7e73435e7cec6e25f0de934bd24c38418c90a64d098689525b2955e7065ead3
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/73" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7e73435e7cec6e25f0de934bd24c38418c90a64d098689525b2955e7065ead3"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a0d5b125357b2096611dc16f0c21549d1eed9c85deb43fefc7338519563fb993
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
	-H "Authorization: Bearer a0d5b125357b2096611dc16f0c21549d1eed9c85deb43fefc7338519563fb993"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 672c212556db90518aef40886bdbad93eef3b651ed73e17f15908dbc0bf36c41
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
    "creator_id": 154,
    "id": 72,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 51,
    "additional_university_ids": [

    ],
    "topic_id": 72,
    "discipline_id": 72,
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
    "chapters_updated_at": "2016-10-19T08:59:42.320Z",
    "updated_at": "2016-10-19T08:59:43.706Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 29,
        "title": "Clever Chapter Title 17",
        "position": 1,
        "updated_at": "2016-10-19T08:59:43.661Z",
        "course_id": 72,
        "author_id": 154,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T08:59:42.320Z",
        "questions_updated_at": "2016-10-19T08:59:42.320Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 30,
        "title": "Clever Chapter Title 18",
        "position": 2,
        "updated_at": "2016-10-19T08:59:43.699Z",
        "course_id": 72,
        "author_id": 154,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-19T08:59:42.320Z",
        "questions_updated_at": "2016-10-19T08:59:42.320Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 154,
        "chapter_id": 29,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.511Z",
        "created_at": "2016-10-19T08:59:43.511Z",
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
        "author_id": 154,
        "chapter_id": 30,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.578Z",
        "created_at": "2016-10-19T08:59:43.578Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 154,
        "chapter_id": 29,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.549Z",
        "created_at": "2016-10-19T08:59:43.549Z",
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
        "author_id": 154,
        "chapter_id": 30,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.614Z",
        "created_at": "2016-10-19T08:59:43.614Z",
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
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 157,
        "chapter_id": 29,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.652Z",
        "created_at": "2016-10-19T08:59:43.652Z",
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
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 158,
        "chapter_id": 30,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:43.689Z",
        "created_at": "2016-10-19T08:59:43.689Z",
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
	-H "Authorization: Bearer 672c212556db90518aef40886bdbad93eef3b651ed73e17f15908dbc0bf36c41"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/85
Content-Type: application/json
Authorization: Bearer 1680ba4c97218e08f7488f0c44ffaa3dfa0557019bad99690624ccaf937c1d85
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
    "creator_id": 185,
    "id": 85,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 64,
    "additional_university_ids": [

    ],
    "topic_id": 85,
    "discipline_id": 85,
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
    "updated_at": "2016-10-19T08:59:45.991Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/85" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1680ba4c97218e08f7488f0c44ffaa3dfa0557019bad99690624ccaf937c1d85"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4e258e49bea836f2ac1468427df2c647bb0effa49e7fcae69bf5a53134de5cb8
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
    "creator_id": 180,
    "id": 82,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 61,
    "additional_university_ids": [

    ],
    "topic_id": 82,
    "discipline_id": 82,
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
    "updated_at": "2016-10-19T08:59:45.603Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e258e49bea836f2ac1468427df2c647bb0effa49e7fcae69bf5a53134de5cb8"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer b32ffb0dbbac7c6032f6e6bf4fed6d36e5c0ee4d4caa1be0e696e5cb627c6817
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
      "id": 2,
      "user_id": 309,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:59:58.463Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 313,
      "feedbackable_id": 68,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:59:58.748Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 317,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:59:59.038Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 321,
      "feedbackable_id": 70,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:59:59.331Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 325,
      "feedbackable_id": 71,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T08:59:59.623Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b32ffb0dbbac7c6032f6e6bf4fed6d36e5c0ee4d4caa1be0e696e5cb627c6817"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 6059bc21c547aa2d01d33539d6245b0204c74c82fc78b7ebd29640556c167626
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
      "user_id": 383,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-19T09:00:03.875Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6059bc21c547aa2d01d33539d6245b0204c74c82fc78b7ebd29640556c167626"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Authorization: Bearer 7538911252f76b66aeab7ad8f1a6e4cf3361c77d05000ca71fbc77f12397b740
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
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Authorization: Bearer 7538911252f76b66aeab7ad8f1a6e4cf3361c77d05000ca71fbc77f12397b740" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/1/metadata
Authorization: Bearer dee1631bfe3660492239eefcd46bd857aa0cbd2441134a0d5f06be8b6b9fb4e3
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
    "id": 1,
    "uploader": {
      "id": 80,
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
      "created_at": "2016-10-19T08:59:32.304Z",
      "updated_at": "2016-10-19T08:59:32.304Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-19T08:59:32.394Z",
    "updated_at": "2016-10-19T08:59:32.394Z",
    "course_id": 50,
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
curl "api.goskive.com/v2/files/1/metadata" -X GET \
	-H "Authorization: Bearer dee1631bfe3660492239eefcd46bd857aa0cbd2441134a0d5f06be8b6b9fb4e3" \
	-H "Content-Type: application/json"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/52/feedbacks
Content-Type: application/json
Authorization: Bearer 3e17455d8af3c3c78416c20526818ef8913813d171c1d28369756e31b75a8ad8
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
      "id": 33,
      "user_id": 497,
      "feedbackable_id": 52,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:11.099Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 496,
      "feedbackable_id": 52,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:11.089Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/52/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e17455d8af3c3c78416c20526818ef8913813d171c1d28369756e31b75a8ad8"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 97a68c83fc57c0dc1422dd60d94ceb997b50e7ea117f05571e8ce11d275586e9
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 591,
      "chapter_id": 124,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:16.855Z",
      "created_at": "2016-10-19T09:00:16.855Z",
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
      "author_id": 594,
      "chapter_id": 125,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:16.986Z",
      "created_at": "2016-10-19T09:00:16.986Z",
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
      "author_id": 597,
      "chapter_id": 126,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:17.116Z",
      "created_at": "2016-10-19T09:00:17.116Z",
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 600,
      "chapter_id": 127,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:17.252Z",
      "created_at": "2016-10-19T09:00:17.252Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 603,
      "chapter_id": 128,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:17.386Z",
      "created_at": "2016-10-19T09:00:17.386Z",
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
	-H "Authorization: Bearer 97a68c83fc57c0dc1422dd60d94ceb997b50e7ea117f05571e8ce11d275586e9"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer e17c33cb6cdb95fb1227d73ee70886f81d20dfa441b6abcce2103cf7c8df2a76
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
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 571,
      "chapter_id": 118,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:15.985Z",
      "created_at": "2016-10-19T09:00:15.985Z",
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
	-H "Authorization: Bearer e17c33cb6cdb95fb1227d73ee70886f81d20dfa441b6abcce2103cf7c8df2a76"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/79/republish
Content-Type: application/json
Authorization: Bearer 28afa413989bdd9cd3383b535e4452e877b24e70316e350ed72f9bd7c36203dd
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/79/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28afa413989bdd9cd3383b535e4452e877b24e70316e350ed72f9bd7c36203dd"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/97/feedbacks
Content-Type: application/json
Authorization: Bearer 42aa55275b199cfc10a9e6286dd59ea716af5bd5636abf75403fc53c43afdd11
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
      "id": 43,
      "user_id": 545,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:14.345Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 544,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:14.334Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/97/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42aa55275b199cfc10a9e6286dd59ea716af5bd5636abf75403fc53c43afdd11"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 7579e3b1cc176443f3ba09c6807b88ba64a7d57e0fca4ceb47f08368352518e5
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 274,
      "chapter_id": 59,
      "position": 56,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:55.083Z",
      "created_at": "2016-10-19T08:59:54.963Z",
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
          "id": 126,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 127,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 265,
      "chapter_id": 56,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:54.232Z",
      "created_at": "2016-10-19T08:59:54.118Z",
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
          "id": 120,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 121,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 268,
      "chapter_id": 57,
      "position": 54,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:54.510Z",
      "created_at": "2016-10-19T08:59:54.393Z",
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
          "id": 122,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 123,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 271,
      "chapter_id": 58,
      "position": 55,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:54.795Z",
      "created_at": "2016-10-19T08:59:54.677Z",
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
          "id": 124,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 125,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 277,
      "chapter_id": 60,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:55.388Z",
      "created_at": "2016-10-19T08:59:55.265Z",
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
          "id": 128,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 129,
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
	-H "Authorization: Bearer 7579e3b1cc176443f3ba09c6807b88ba64a7d57e0fca4ceb47f08368352518e5"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer e581c2f92137c5d395b74dd80f0d37808085c3ad4579009185d2d8ef577630cb
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 245,
      "chapter_id": 50,
      "position": 47,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:52.360Z",
      "created_at": "2016-10-19T08:59:52.246Z",
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
          "id": 108,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 109,
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
	-H "Authorization: Bearer e581c2f92137c5d395b74dd80f0d37808085c3ad4579009185d2d8ef577630cb"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/49/republish
Content-Type: application/json
Authorization: Bearer ba7cc922862c5e4b298fc53ae1c0a1239e1b2f402b519221d8c5a46d8a66e824
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba7cc922862c5e4b298fc53ae1c0a1239e1b2f402b519221d8c5a46d8a66e824"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9e390296669577819f10867cd8e30d910be9b95137a46235b38071155a0f9418
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":49,"published":false}}
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
    "creator_id": 79,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 27,
    "additional_university_ids": [

    ],
    "topic_id": 49,
    "discipline_id": 49,
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
    "updated_at": "2016-10-19T08:59:32.257Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":49,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e390296669577819f10867cd8e30d910be9b95137a46235b38071155a0f9418"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cfd6ae365ca1f4d30d43201c34a4554f34a2259288143c1b9e934fb88176938c
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
      "creator_id": 56,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-21",
      "html_url": "https://goskive.com/course/fu-course-21",
      "slug": "fu-course-21",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 30,
      "discipline_id": 30,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 21",
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
      "updated_at": "2016-10-19T08:59:29.970Z",
      "shortname": "fu-course-21"
    },
    {
      "creator_id": 56,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-22",
      "html_url": "https://goskive.com/course/fu-course-22",
      "slug": "fu-course-22",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 31,
      "discipline_id": 31,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 22",
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
      "updated_at": "2016-10-19T08:59:30.009Z",
      "shortname": "fu-course-22"
    },
    {
      "creator_id": 57,
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 32,
      "discipline_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
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
      "updated_at": "2016-10-19T08:59:30.056Z",
      "shortname": "fu-course-23"
    },
    {
      "creator_id": 57,
      "id": 33,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 33,
      "discipline_id": 33,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
      "chapters_updated_at": "2016-10-19T08:59:30.348Z",
      "updated_at": "2016-10-19T08:59:30.359Z",
      "shortname": "fu-course-24"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfd6ae365ca1f4d30d43201c34a4554f34a2259288143c1b9e934fb88176938c"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4332034e7759b533c95d2e3ec97a53413d77408462c77ec1dad9bebab3cf6521
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
      "creator_id": 63,
      "id": 34,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-25",
      "html_url": "https://goskive.com/course/fu-course-25",
      "slug": "fu-course-25",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "topic_id": 34,
      "discipline_id": 34,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 25",
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
      "updated_at": "2016-10-19T08:59:30.580Z",
      "shortname": "fu-course-25"
    },
    {
      "creator_id": 63,
      "id": 35,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-26",
      "html_url": "https://goskive.com/course/fu-course-26",
      "slug": "fu-course-26",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "topic_id": 35,
      "discipline_id": 35,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 26",
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
      "updated_at": "2016-10-19T08:59:30.619Z",
      "shortname": "fu-course-26"
    },
    {
      "creator_id": 64,
      "id": 36,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "topic_id": 36,
      "discipline_id": 36,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
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
      "updated_at": "2016-10-19T08:59:30.669Z",
      "shortname": "fu-course-27"
    },
    {
      "creator_id": 64,
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "topic_id": 37,
      "discipline_id": 37,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
      "updated_at": "2016-10-19T08:59:30.711Z",
      "shortname": "fu-course-28"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4332034e7759b533c95d2e3ec97a53413d77408462c77ec1dad9bebab3cf6521"
```
