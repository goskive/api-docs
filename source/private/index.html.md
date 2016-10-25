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
DELETE /v2/chapters/105
Content-Type: application/json
Authorization: Bearer cfd63468ed706e0e3f28291c3658e5b2d96a27ca00234be12c6dde3d5196d047
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/105" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfd63468ed706e0e3f28291c3658e5b2d96a27ca00234be12c6dde3d5196d047"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/104
Content-Type: application/json
Authorization: Bearer 4e9f9f623c7e8954876d715254bf5782b1fab97ce8023b199975f882b6328dd9
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
    "id": 104,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T20:44:41.156Z",
    "course_id": 119,
    "author_id": 459,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T20:44:40.495Z",
    "questions_updated_at": "2016-10-25T20:44:40.495Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 462,
        "chapter_id": 104,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:41.094Z",
        "created_at": "2016-10-25T20:44:41.094Z",
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
        "author_id": 463,
        "chapter_id": 104,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:41.135Z",
        "created_at": "2016-10-25T20:44:41.135Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 460,
        "chapter_id": 104,
        "position": 64,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:40.754Z",
        "created_at": "2016-10-25T20:44:40.604Z",
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
            "id": 138,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 139,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 461,
        "chapter_id": 104,
        "position": 65,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:41.009Z",
        "created_at": "2016-10-25T20:44:40.850Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/104" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e9f9f623c7e8954876d715254bf5782b1fab97ce8023b199975f882b6328dd9"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/111
Content-Type: application/json
Authorization: Bearer 1464f6b04adbeddad316d135f51a70a020701c2b25d16e2a15898475c5f5246b
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
    "id": 111,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T20:44:42.712Z",
    "course_id": 126,
    "author_id": 483,
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
curl "api.goskive.com/v2/chapters/111" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1464f6b04adbeddad316d135f51a70a020701c2b25d16e2a15898475c5f5246b"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/21
Content-Type: application/json
Authorization: Bearer 26eafc3b27943d309b433da20039f3f3bc8f72ac5dd72691234769f705510d4d
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26eafc3b27943d309b433da20039f3f3bc8f72ac5dd72691234769f705510d4d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 4d038c10931c936e456dae589618376677cd457bfad230987dad1a38f2ed136f
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
      "id": 32,
      "author_id": 757,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:05.122Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 759,
      "reply_to_id": 32,
      "created_at": "2016-10-25T20:45:05.207Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 761,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:05.291Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 763,
      "reply_to_id": 34,
      "created_at": "2016-10-25T20:45:05.370Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 765,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:05.451Z",
      "status": "reported",
      "subject_id": 240,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 767,
      "reply_to_id": 36,
      "created_at": "2016-10-25T20:45:05.529Z",
      "status": "published",
      "subject_id": 241,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 769,
      "reply_to_id": 36,
      "created_at": "2016-10-25T20:45:05.608Z",
      "status": "published",
      "subject_id": 242,
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
	-H "Authorization: Bearer 4d038c10931c936e456dae589618376677cd457bfad230987dad1a38f2ed136f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 82698d223432f6a8344a3e5488e61d4bbb3f256053a127b2f752211b9bf9db91
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
      "id": 46,
      "author_id": 787,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:06.344Z",
      "status": "published",
      "subject_id": 250,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 789,
      "reply_to_id": 46,
      "created_at": "2016-10-25T20:45:06.424Z",
      "status": "published",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 791,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:06.529Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 793,
      "reply_to_id": 48,
      "created_at": "2016-10-25T20:45:06.608Z",
      "status": "published",
      "subject_id": 253,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 795,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:06.688Z",
      "status": "reported",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 797,
      "reply_to_id": 50,
      "created_at": "2016-10-25T20:45:06.766Z",
      "status": "published",
      "subject_id": 255,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 799,
      "reply_to_id": 50,
      "created_at": "2016-10-25T20:45:06.846Z",
      "status": "published",
      "subject_id": 256,
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
	-H "Authorization: Bearer 82698d223432f6a8344a3e5488e61d4bbb3f256053a127b2f752211b9bf9db91"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer a694bac9abe9bbaee301104a67d5c365822a9463dac187f1d9e0a11b50a6119c
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
      "id": 54,
      "author_id": 804,
      "reply_to_id": 53,
      "created_at": "2016-10-25T20:45:07.065Z",
      "status": "published",
      "subject_id": 258,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 56,
      "author_id": 808,
      "reply_to_id": 55,
      "created_at": "2016-10-25T20:45:07.220Z",
      "status": "published",
      "subject_id": 260,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 58,
      "author_id": 812,
      "reply_to_id": 57,
      "created_at": "2016-10-25T20:45:07.378Z",
      "status": "published",
      "subject_id": 262,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 814,
      "reply_to_id": 57,
      "created_at": "2016-10-25T20:45:07.458Z",
      "status": "published",
      "subject_id": 263,
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
	-H "Authorization: Bearer a694bac9abe9bbaee301104a67d5c365822a9463dac187f1d9e0a11b50a6119c"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 90a0e13c2b23aa7b3c51ad732ff9dcf49a0a033c316dea82a2c7032b6bcca8f3
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
      "id": 43,
      "author_id": 780,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:45:06.062Z",
      "status": "reported",
      "subject_id": 247,
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
	-H "Authorization: Bearer 90a0e13c2b23aa7b3c51ad732ff9dcf49a0a033c316dea82a2c7032b6bcca8f3"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/24/republish
Content-Type: application/json
Authorization: Bearer 2c44f89aede24d82d3f40804ea1d1b7958076b648c370d2c7285f6a8a02f56a8
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/24/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c44f89aede24d82d3f40804ea1d1b7958076b648c370d2c7285f6a8a02f56a8"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/41/chapters
Content-Type: application/json
Authorization: Bearer 4ebb4c4ec8b2911c80aa82d9bd2bc87582cd90b76166ff2267567a62513007f4
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
    "id": 41,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:44:14.512Z",
    "course_id": 41,
    "author_id": 143,
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
curl "api.goskive.com/v2/courses/41/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ebb4c4ec8b2911c80aa82d9bd2bc87582cd90b76166ff2267567a62513007f4"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ee9b61edc84827a0810a8703df4438ac2eb529e922f003e053bdef86c7c6b4eb
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
    "id": 42,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:44:14.637Z",
    "course_id": 42,
    "author_id": 145,
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
	-H "Authorization: Bearer ee9b61edc84827a0810a8703df4438ac2eb529e922f003e053bdef86c7c6b4eb"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5e59ed0ff39151f7eb1bcd21c07a3d18e43da8257a43c916ffd923e16bb7910a
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
      "id": 26,
      "title": "Clever Chapter Title 23",
      "position": 1,
      "updated_at": "2016-10-25T20:44:12.944Z",
      "course_id": 33,
      "author_id": 111,
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
      "id": 27,
      "title": "Clever Chapter Title 24",
      "position": 2,
      "updated_at": "2016-10-25T20:44:12.966Z",
      "course_id": 33,
      "author_id": 112,
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
      "id": 28,
      "title": "Clever Chapter Title 25",
      "position": 3,
      "updated_at": "2016-10-25T20:44:13.209Z",
      "course_id": 33,
      "author_id": 113,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T20:44:12.871Z",
      "questions_updated_at": "2016-10-25T20:44:12.871Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e59ed0ff39151f7eb1bcd21c07a3d18e43da8257a43c916ffd923e16bb7910a"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f10f331d89bdc4dc37fd94c879fcf5b050bfbf478446a93fff595cb400e59dcd
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
      "id": 29,
      "title": "Clever Chapter Title 26",
      "position": 1,
      "updated_at": "2016-10-25T20:44:13.339Z",
      "course_id": 34,
      "author_id": 118,
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
      "id": 30,
      "title": "Clever Chapter Title 27",
      "position": 2,
      "updated_at": "2016-10-25T20:44:13.361Z",
      "course_id": 34,
      "author_id": 119,
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
      "id": 31,
      "title": "Clever Chapter Title 28",
      "position": 3,
      "updated_at": "2016-10-25T20:44:13.382Z",
      "course_id": 34,
      "author_id": 120,
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
	-H "Authorization: Bearer f10f331d89bdc4dc37fd94c879fcf5b050bfbf478446a93fff595cb400e59dcd"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ff6b67bf146e87e571a09b6a6a26eb46b160d5b5af042cf3f088e7dc7bc2561e
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
	-H "Authorization: Bearer ff6b67bf146e87e571a09b6a6a26eb46b160d5b5af042cf3f088e7dc7bc2561e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/219
Content-Type: application/json
Authorization: Bearer 72c1cebf7cd60e9ed10ad5149f267a667569e0531cdf7aa4d648338acc762b3c
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/219" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72c1cebf7cd60e9ed10ad5149f267a667569e0531cdf7aa4d648338acc762b3c"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer a3e6f6e511667d525e5e02f79818c9b38552723c4d492a7925128c1a2dddb877
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
    "creator_id": 721,
    "id": 223,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 202,
    "additional_university_ids": [

    ],
    "topic_id": 235,
    "discipline_id": 236,
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
    "chapters_updated_at": "2016-10-25T20:45:02.247Z",
    "updated_at": "2016-10-25T20:45:03.626Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 166,
        "title": "Clever Chapter Title 142",
        "position": 1,
        "updated_at": "2016-10-25T20:45:03.583Z",
        "course_id": 223,
        "author_id": 721,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T20:45:02.247Z",
        "questions_updated_at": "2016-10-25T20:45:02.247Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 167,
        "title": "Clever Chapter Title 143",
        "position": 2,
        "updated_at": "2016-10-25T20:45:03.620Z",
        "course_id": 223,
        "author_id": 721,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T20:45:02.247Z",
        "questions_updated_at": "2016-10-25T20:45:02.247Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 721,
        "chapter_id": 166,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.433Z",
        "created_at": "2016-10-25T20:45:03.433Z",
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
        "author_id": 721,
        "chapter_id": 167,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.500Z",
        "created_at": "2016-10-25T20:45:03.500Z",
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
        "author_id": 721,
        "chapter_id": 166,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.470Z",
        "created_at": "2016-10-25T20:45:03.470Z",
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
        "author_id": 721,
        "chapter_id": 167,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.538Z",
        "created_at": "2016-10-25T20:45:03.538Z",
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
        "author_id": 724,
        "chapter_id": 166,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.574Z",
        "created_at": "2016-10-25T20:45:03.574Z",
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
        "author_id": 725,
        "chapter_id": 167,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:03.610Z",
        "created_at": "2016-10-25T20:45:03.610Z",
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
	-H "Authorization: Bearer a3e6f6e511667d525e5e02f79818c9b38552723c4d492a7925128c1a2dddb877"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/206
Content-Type: application/json
Authorization: Bearer 831474f371229edb080d5c76fd620354123e56dd24a6c2bd81ece48090ba098f
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
    "creator_id": 675,
    "id": 206,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 185,
    "additional_university_ids": [

    ],
    "topic_id": 218,
    "discipline_id": 219,
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
    "updated_at": "2016-10-25T20:44:55.847Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/206" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 831474f371229edb080d5c76fd620354123e56dd24a6c2bd81ece48090ba098f"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6191787e793593ca7a95c9b83d83775e084afeb8e777e1ab6c4d0a4b93a4dac9
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
    "creator_id": 679,
    "id": 208,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 187,
    "additional_university_ids": [

    ],
    "topic_id": 220,
    "discipline_id": 221,
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
    "updated_at": "2016-10-25T20:44:56.092Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6191787e793593ca7a95c9b83d83775e084afeb8e777e1ab6c4d0a4b93a4dac9"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 4cc00d720ecd79d7dbcd3984b6d26c2df162c45ca7846a7e061f8aaa9c5be610
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
      "id": 19,
      "user_id": 344,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:30.589Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 20,
      "user_id": 348,
      "feedbackable_id": 48,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:30.925Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 352,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:31.268Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 356,
      "feedbackable_id": 50,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:31.617Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 360,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T20:44:31.957Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cc00d720ecd79d7dbcd3984b6d26c2df162c45ca7846a7e061f8aaa9c5be610"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 0d62425993efa06a260321fbd58a8c90e6d124dc9c427f75177aba205b55f834
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
      "id": 28,
      "user_id": 381,
      "feedbackable_id": 56,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T20:44:33.977Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d62425993efa06a260321fbd58a8c90e6d124dc9c427f75177aba205b55f834"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer 8874352aaef171c221604a4b312a3f7100a10c37af615a5398536746723d6b4f
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8874352aaef171c221604a4b312a3f7100a10c37af615a5398536746723d6b4f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer bed27d1ec7511a6d78b8c8b4bb5029a05a9bc0e1221882211cb24d704d9bfb37
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
    "id": 11,
    "uploader": {
      "id": 939,
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
      "created_at": "2016-10-25T20:45:18.506Z",
      "updated_at": "2016-10-25T20:45:18.506Z"
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
    "created_at": "2016-10-25T20:45:18.577Z",
    "updated_at": "2016-10-25T20:45:18.577Z",
    "course_id": 301,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bed27d1ec7511a6d78b8c8b4bb5029a05a9bc0e1221882211cb24d704d9bfb37"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/36/feedbacks
Content-Type: application/json
Authorization: Bearer 00647cfbe411505b68b28eb9633417689df5317f5ab49c6d06c4108df68923b3
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
      "user_id": 497,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:43.276Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 496,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:43.265Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00647cfbe411505b68b28eb9633417689df5317f5ab49c6d06c4108df68923b3"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5d8c23249cd62d290238073de6db79dfe9a0f5adddf2db901480c90ec566418d
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 548,
      "chapter_id": 128,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:46.665Z",
      "created_at": "2016-10-25T20:44:46.665Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 551,
      "chapter_id": 129,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:46.802Z",
      "created_at": "2016-10-25T20:44:46.802Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 554,
      "chapter_id": 130,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:46.968Z",
      "created_at": "2016-10-25T20:44:46.968Z",
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 557,
      "chapter_id": 131,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:47.105Z",
      "created_at": "2016-10-25T20:44:47.105Z",
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 560,
      "chapter_id": 132,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:47.243Z",
      "created_at": "2016-10-25T20:44:47.243Z",
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
	-H "Authorization: Bearer 5d8c23249cd62d290238073de6db79dfe9a0f5adddf2db901480c90ec566418d"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer b23733d328031b3e4a843a105d93581a5c9fa268654cf357b933789a7655dfaa
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 592,
      "chapter_id": 142,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:48.669Z",
      "created_at": "2016-10-25T20:44:48.669Z",
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
	-H "Authorization: Bearer b23733d328031b3e4a843a105d93581a5c9fa268654cf357b933789a7655dfaa"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/republish
Content-Type: application/json
Authorization: Bearer a1b75d2a2c0d3335e887b528e3df9cc1a31236d50eea794489b68da623bb702d
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1b75d2a2c0d3335e887b528e3df9cc1a31236d50eea794489b68da623bb702d"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/4/feedbacks
Content-Type: application/json
Authorization: Bearer cc1d912b02fb747fb7f1679f4cd333e4e670770c321eb2082dbec628ccbac23b
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
      "id": 4,
      "user_id": 16,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:05.009Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 15,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:04.999Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/4/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc1d912b02fb747fb7f1679f4cd333e4e670770c321eb2082dbec628ccbac23b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer ab3409af96e29d2467dee5e8a5e2c83b1bfc7d8f7aad3731924277ac173cb4a3
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
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 859,
      "chapter_id": 179,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:12.214Z",
      "created_at": "2016-10-25T20:45:12.101Z",
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
          "id": 239,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 240,
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
      "author_id": 853,
      "chapter_id": 177,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:11.681Z",
      "created_at": "2016-10-25T20:45:11.569Z",
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
    },
    {
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 856,
      "chapter_id": 178,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:11.948Z",
      "created_at": "2016-10-25T20:45:11.837Z",
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
          "id": 237,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 238,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 119,
      "obfuscated_id": "JRh8sWka24Y",
      "author_id": 862,
      "chapter_id": 180,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:12.489Z",
      "created_at": "2016-10-25T20:45:12.364Z",
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
          "id": 241,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 242,
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
      "author_id": 865,
      "chapter_id": 181,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:12.748Z",
      "created_at": "2016-10-25T20:45:12.645Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab3409af96e29d2467dee5e8a5e2c83b1bfc7d8f7aad3731924277ac173cb4a3"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 1604eb3cc16ff747b6ed2240b052db798cf89b647c2be090178d395a99a641eb
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
      "id": 125,
      "obfuscated_id": "K6zw0Yc6Me8",
      "author_id": 881,
      "chapter_id": 186,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:45:14.140Z",
      "created_at": "2016-10-25T20:45:14.036Z",
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
          "id": 253,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 254,
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
	-H "Authorization: Bearer 1604eb3cc16ff747b6ed2240b052db798cf89b647c2be090178d395a99a641eb"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/113/republish
Content-Type: application/json
Authorization: Bearer 79ab70c0f9a440cc8e7e1c8280b019d295f6353b28e0208dbdd4cdf15e4817a8
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/113/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79ab70c0f9a440cc8e7e1c8280b019d295f6353b28e0208dbdd4cdf15e4817a8"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1143b58ecd664596d0ee65cb3718967e13e3e24c22bae2840c92b62c557b86e9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":210,"published":false}}
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
    "creator_id": 645,
    "id": 198,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 177,
    "additional_university_ids": [

    ],
    "topic_id": 210,
    "discipline_id": 211,
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
    "updated_at": "2016-10-25T20:44:53.192Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":210,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1143b58ecd664596d0ee65cb3718967e13e3e24c22bae2840c92b62c557b86e9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1c85386e283a060af95d1aeb3206401aa726a0780c1481e6eb6b2640bd6c86e4
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
      "creator_id": 606,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 115",
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
      "updated_at": "2016-10-25T20:44:49.578Z",
      "shortname": "fu-course-115"
    },
    {
      "creator_id": 606,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-116",
      "html_url": "https://goskive.com/course/fu-course-116",
      "slug": "fu-course-116",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 116",
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
      "updated_at": "2016-10-25T20:44:49.614Z",
      "shortname": "fu-course-116"
    },
    {
      "creator_id": 607,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-117",
      "html_url": "https://goskive.com/course/fu-course-117",
      "slug": "fu-course-117",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 117",
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
      "updated_at": "2016-10-25T20:44:49.661Z",
      "shortname": "fu-course-117"
    },
    {
      "creator_id": 607,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-118",
      "html_url": "https://goskive.com/course/fu-course-118",
      "slug": "fu-course-118",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 118",
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
      "chapters_updated_at": "2016-10-25T20:44:49.938Z",
      "updated_at": "2016-10-25T20:44:49.944Z",
      "shortname": "fu-course-118"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c85386e283a060af95d1aeb3206401aa726a0780c1481e6eb6b2640bd6c86e4"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ae65692cd9d752f5998bcb1ed90ca866cebbd1499157b78ffd2142e6b582b61c
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
      "creator_id": 613,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
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
      "updated_at": "2016-10-25T20:44:50.142Z",
      "shortname": "fu-course-119"
    },
    {
      "creator_id": 613,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 182,
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
      "updated_at": "2016-10-25T20:44:50.182Z",
      "shortname": "fu-course-120"
    },
    {
      "creator_id": 614,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-121",
      "html_url": "https://goskive.com/course/fu-course-121",
      "slug": "fu-course-121",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 183,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T20:44:50.231Z",
      "shortname": "fu-course-121"
    },
    {
      "creator_id": 614,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 183,
      "discipline_id": 184,
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
      "updated_at": "2016-10-25T20:44:50.297Z",
      "shortname": "fu-course-122"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae65692cd9d752f5998bcb1ed90ca866cebbd1499157b78ffd2142e6b582b61c"
```
