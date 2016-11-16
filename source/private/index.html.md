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
DELETE /v2/chapters/123
Content-Type: application/json
Authorization: Bearer e33e5fd086575fa59131fa4c2b260866d80ed5002321dd2056bbdac95f9c6b59
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/123" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e33e5fd086575fa59131fa4c2b260866d80ed5002321dd2056bbdac95f9c6b59"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/119
Content-Type: application/json
Authorization: Bearer 52ada63635b1d55ad60ae5695b7d0ca55834da473621cc386d0798eb747e7c40
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
    "id": 119,
    "updated_at": "2016-11-16T17:23:53.235Z",
    "course_id": 236,
    "author_id": 668,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-16T17:23:52.705Z",
    "questions_updated_at": "2016-11-16T17:23:52.705Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 671,
        "chapter_id": 119,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:53.181Z",
        "created_at": "2016-11-16T17:23:53.181Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 672,
        "chapter_id": 119,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:53.218Z",
        "created_at": "2016-11-16T17:23:53.218Z",
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
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 669,
        "chapter_id": 119,
        "position": 82,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:52.919Z",
        "created_at": "2016-11-16T17:23:52.811Z",
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
            "id": 193,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 194,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 670,
        "chapter_id": 119,
        "position": 83,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:53.113Z",
        "created_at": "2016-11-16T17:23:52.993Z",
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
            "id": 195,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 196,
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
curl "api.goskive.com/v2/chapters/119" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52ada63635b1d55ad60ae5695b7d0ca55834da473621cc386d0798eb747e7c40"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/126
Content-Type: application/json
Authorization: Bearer c08739bfa500445c8057296008a30ad94f3d64c1849ada2e25599ff6ba1cc6c5
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
    "id": 126,
    "updated_at": "2016-11-16T17:23:55.181Z",
    "course_id": 243,
    "author_id": 697,
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
curl "api.goskive.com/v2/chapters/126" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c08739bfa500445c8057296008a30ad94f3d64c1849ada2e25599ff6ba1cc6c5"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/43
Content-Type: application/json
Authorization: Bearer 9606045f13b76409ef5c3962ba36b36334a5a5f78c24f813ba1d7aeb93428ec5
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/43" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9606045f13b76409ef5c3962ba36b36334a5a5f78c24f813ba1d7aeb93428ec5"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 4e475728971cc28a572e2a8b34c2dfc925ee4e3d7a712da4c2fbb44425aa7552
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
      "author_id": 41,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:22:58.453Z",
      "status": "published",
      "subject_id": 17,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 43,
      "reply_to_id": 14,
      "created_at": "2016-11-16T17:22:58.536Z",
      "status": "published",
      "subject_id": 18,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 45,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:22:58.611Z",
      "status": "published",
      "subject_id": 19,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 47,
      "reply_to_id": 16,
      "created_at": "2016-11-16T17:22:58.685Z",
      "status": "published",
      "subject_id": 20,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 49,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:22:58.792Z",
      "status": "reported",
      "subject_id": 21,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 51,
      "reply_to_id": 18,
      "created_at": "2016-11-16T17:22:58.868Z",
      "status": "published",
      "subject_id": 22,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 53,
      "reply_to_id": 18,
      "created_at": "2016-11-16T17:22:58.949Z",
      "status": "published",
      "subject_id": 23,
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
	-H "Authorization: Bearer 4e475728971cc28a572e2a8b34c2dfc925ee4e3d7a712da4c2fbb44425aa7552"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 73fcb20ad4553386d1252c72eeeb4b58c978f3723c42f2ed81604d2c2654fab9
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
      "id": 35,
      "author_id": 86,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:00.254Z",
      "status": "published",
      "subject_id": 38,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 88,
      "reply_to_id": 35,
      "created_at": "2016-11-16T17:23:00.331Z",
      "status": "published",
      "subject_id": 39,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 90,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:00.411Z",
      "status": "published",
      "subject_id": 40,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 92,
      "reply_to_id": 37,
      "created_at": "2016-11-16T17:23:00.488Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 94,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:00.582Z",
      "status": "reported",
      "subject_id": 42,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 96,
      "reply_to_id": 39,
      "created_at": "2016-11-16T17:23:00.666Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 98,
      "reply_to_id": 39,
      "created_at": "2016-11-16T17:23:00.749Z",
      "status": "published",
      "subject_id": 44,
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
	-H "Authorization: Bearer 73fcb20ad4553386d1252c72eeeb4b58c978f3723c42f2ed81604d2c2654fab9"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer d3b60973f72d1ec56909d8825ef90cfcdcc7247c657f396cd90ac11529201a17
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
      "id": 29,
      "author_id": 73,
      "reply_to_id": 28,
      "created_at": "2016-11-16T17:22:59.739Z",
      "status": "published",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 77,
      "reply_to_id": 30,
      "created_at": "2016-11-16T17:22:59.895Z",
      "status": "published",
      "subject_id": 34,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 81,
      "reply_to_id": 32,
      "created_at": "2016-11-16T17:23:00.052Z",
      "status": "published",
      "subject_id": 36,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 83,
      "reply_to_id": 32,
      "created_at": "2016-11-16T17:23:00.130Z",
      "status": "published",
      "subject_id": 37,
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
	-H "Authorization: Bearer d3b60973f72d1ec56909d8825ef90cfcdcc7247c657f396cd90ac11529201a17"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 692a7205020c746a6ef7326c44b6e274253151c7d737f47955a95f53031b6aa5
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
      "id": 25,
      "author_id": 64,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:22:59.388Z",
      "status": "reported",
      "subject_id": 28,
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
	-H "Authorization: Bearer 692a7205020c746a6ef7326c44b6e274253151c7d737f47955a95f53031b6aa5"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer 87b530edf913c0203109117de999093bd49f7a4ad1f1e8e767bb8f3dff8b1dd5
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87b530edf913c0203109117de999093bd49f7a4ad1f1e8e767bb8f3dff8b1dd5"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 31409186bb29bfb54a6f9e70bf67a698866b2a51df7180b7e0eba89568e95a03
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
    "id": 52,
    "updated_at": "2016-11-16T17:23:25.128Z",
    "course_id": 150,
    "author_id": 382,
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
	-H "Authorization: Bearer 31409186bb29bfb54a6f9e70bf67a698866b2a51df7180b7e0eba89568e95a03"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/152/chapters
Content-Type: application/json
Authorization: Bearer 974f9ce8ffbc8c76466cc51de297173089a2fdd800e7a5321064034684d21c10
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
    "id": 53,
    "updated_at": "2016-11-16T17:23:25.395Z",
    "course_id": 152,
    "author_id": 386,
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
curl "api.goskive.com/v2/courses/152/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 974f9ce8ffbc8c76466cc51de297173089a2fdd800e7a5321064034684d21c10"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7fd6df5617578ee3fe966230260b0ca7b8c07a6578212668c2c44918f4403154
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
      "id": 54,
      "updated_at": "2016-11-16T17:23:25.556Z",
      "course_id": 153,
      "author_id": 388,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 39",
      "position": 1
    },
    {
      "id": 55,
      "updated_at": "2016-11-16T17:23:25.579Z",
      "course_id": 153,
      "author_id": 389,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 40",
      "position": 2
    },
    {
      "id": 56,
      "updated_at": "2016-11-16T17:23:25.823Z",
      "course_id": 153,
      "author_id": 390,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-16T17:23:25.484Z",
      "questions_updated_at": "2016-11-16T17:23:25.484Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 41",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7fd6df5617578ee3fe966230260b0ca7b8c07a6578212668c2c44918f4403154"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 268fd64cbc60771f93f37061fc5da846aae9ff0ed081096d886c88c71dc75ff7
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
      "id": 57,
      "updated_at": "2016-11-16T17:23:26.005Z",
      "course_id": 154,
      "author_id": 395,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 42",
      "position": 1
    },
    {
      "id": 58,
      "updated_at": "2016-11-16T17:23:26.032Z",
      "course_id": 154,
      "author_id": 396,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 43",
      "position": 2
    },
    {
      "id": 59,
      "updated_at": "2016-11-16T17:23:26.057Z",
      "course_id": 154,
      "author_id": 397,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 44",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 268fd64cbc60771f93f37061fc5da846aae9ff0ed081096d886c88c71dc75ff7"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/209
Content-Type: application/json
Authorization: Bearer 33fefb5d21ce41cde5bc3a374433ed5e4aa4281babc0e69e134eab38e1ca22d6
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/209" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33fefb5d21ce41cde5bc3a374433ed5e4aa4281babc0e69e134eab38e1ca22d6"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 80c71698e7a795f9fb3034e7dc68eb888758034267efc00ed7469ba9cedf7ee6
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
	-H "Authorization: Bearer 80c71698e7a795f9fb3034e7dc68eb888758034267efc00ed7469ba9cedf7ee6"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4d43aacb5c213e1487f384202217caf21b6e8becca5aa3d13f1994bcf3fd58fe
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
    "creator_id": 581,
    "id": 206,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 191,
    "additional_university_ids": [

    ],
    "discipline_id": 216,
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
    "chapters_updated_at": "2016-11-16T17:23:41.344Z",
    "updated_at": "2016-11-16T17:23:42.777Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 581,
        "chapter_id": 105,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.579Z",
        "created_at": "2016-11-16T17:23:42.579Z",
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
        "author_id": 581,
        "chapter_id": 106,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.647Z",
        "created_at": "2016-11-16T17:23:42.647Z",
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
        "author_id": 581,
        "chapter_id": 105,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.617Z",
        "created_at": "2016-11-16T17:23:42.617Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 581,
        "chapter_id": 106,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.685Z",
        "created_at": "2016-11-16T17:23:42.685Z",
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
        "author_id": 584,
        "chapter_id": 105,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.721Z",
        "created_at": "2016-11-16T17:23:42.721Z",
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
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 585,
        "chapter_id": 106,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:42.759Z",
        "created_at": "2016-11-16T17:23:42.759Z",
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
        "id": 105,
        "updated_at": "2016-11-16T17:23:42.731Z",
        "course_id": 206,
        "author_id": 581,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-16T17:23:41.344Z",
        "questions_updated_at": "2016-11-16T17:23:41.344Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 90",
        "position": 1
      },
      {
        "id": 106,
        "updated_at": "2016-11-16T17:23:42.769Z",
        "course_id": 206,
        "author_id": 581,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-16T17:23:41.344Z",
        "questions_updated_at": "2016-11-16T17:23:41.344Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 91",
        "position": 2
      }
    ],
    "topic_id": 215,
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
	-H "Authorization: Bearer 4d43aacb5c213e1487f384202217caf21b6e8becca5aa3d13f1994bcf3fd58fe"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/222
Content-Type: application/json
Authorization: Bearer 33fd25dd26499abb966149e99849b0473e50235a515ee28b2c7120bbfa71ff43
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
    "creator_id": 625,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "discipline_id": 232,
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
    "updated_at": "2016-11-16T17:23:48.162Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 231,
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
curl "api.goskive.com/v2/courses/222" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33fd25dd26499abb966149e99849b0473e50235a515ee28b2c7120bbfa71ff43"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer dabc9531bbb923e1082cce0460fa5d150b332e4d1be6349c4f52fa1f4d70820a
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
    "creator_id": 620,
    "id": 219,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 204,
    "additional_university_ids": [

    ],
    "discipline_id": 229,
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
    "updated_at": "2016-11-16T17:23:47.671Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 228,
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
	-H "Authorization: Bearer dabc9531bbb923e1082cce0460fa5d150b332e4d1be6349c4f52fa1f4d70820a"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 6ea8e7b50fc9c2b7332f2aa83ea611b7c266e6e94418f4c9420bdbbf494f33c3
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
      "id": 26,
      "user_id": 775,
      "feedbackable_id": 110,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:00.252Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 779,
      "feedbackable_id": 111,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:00.540Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 783,
      "feedbackable_id": 112,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:00.834Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 787,
      "feedbackable_id": 113,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:01.164Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 791,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-16T17:24:01.466Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ea8e7b50fc9c2b7332f2aa83ea611b7c266e6e94418f4c9420bdbbf494f33c3"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer acfea653230b53587782e71286f8746bbfd469bbc1f43a4a1f9eafc5aa21eceb
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
      "id": 35,
      "user_id": 812,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-16T17:24:02.997Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer acfea653230b53587782e71286f8746bbfd469bbc1f43a4a1f9eafc5aa21eceb"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 748bc3d4c73baba67ba2c33f6c5e280ec0f98061d9c138863dd4b98c4579f2da
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 748bc3d4c73baba67ba2c33f6c5e280ec0f98061d9c138863dd4b98c4579f2da"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer 4de4a1787cf8212445ac457cea761a4ca31bcb59761e212962c669bf02bbeaa0
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
    "id": 13,
    "uploader": {
      "id": 549,
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
      "created_at": "2016-11-16T17:23:38.428Z",
      "updated_at": "2016-11-16T17:23:38.428Z"
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
    "created_at": "2016-11-16T17:23:38.528Z",
    "updated_at": "2016-11-16T17:23:38.528Z",
    "course_id": 197,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4de4a1787cf8212445ac457cea761a4ca31bcb59761e212962c669bf02bbeaa0"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/8/feedbacks
Content-Type: application/json
Authorization: Bearer 74a0f610be746f2b1343641264b12afeaa4a40379f91c4ab26086a0ca6662dbe
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
      "id": 6,
      "user_id": 251,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:15.100Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 250,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:15.090Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74a0f610be746f2b1343641264b12afeaa4a40379f91c4ab26086a0ca6662dbe"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 253247cbe3f1af8f038ddc713b0783801d22558e2f660595e90332d1af887564
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
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 933,
      "chapter_id": 182,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:11.710Z",
      "created_at": "2016-11-16T17:24:11.710Z",
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
      "id": 83,
      "obfuscated_id": "FCSR-nKROLo",
      "author_id": 936,
      "chapter_id": 183,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:11.840Z",
      "created_at": "2016-11-16T17:24:11.840Z",
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
      "id": 84,
      "obfuscated_id": "Hu6DTUHzhWo",
      "author_id": 939,
      "chapter_id": 184,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:11.970Z",
      "created_at": "2016-11-16T17:24:11.970Z",
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
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 942,
      "chapter_id": 185,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:12.103Z",
      "created_at": "2016-11-16T17:24:12.103Z",
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
      "author_id": 945,
      "chapter_id": 186,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:12.274Z",
      "created_at": "2016-11-16T17:24:12.274Z",
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
	-H "Authorization: Bearer 253247cbe3f1af8f038ddc713b0783801d22558e2f660595e90332d1af887564"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 75900a27c7fea7ede43291ca5cf27250d93bf064f79a65549c568a000a4dfaed
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
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 961,
      "chapter_id": 191,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:24:12.993Z",
      "created_at": "2016-11-16T17:24:12.993Z",
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
	-H "Authorization: Bearer 75900a27c7fea7ede43291ca5cf27250d93bf064f79a65549c568a000a4dfaed"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/94/republish
Content-Type: application/json
Authorization: Bearer 042f4977d040c09397020c3184d28a653da31af8bcd67d084d475d7c8f4c204f
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/94/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 042f4977d040c09397020c3184d28a653da31af8bcd67d084d475d7c8f4c204f"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/124/feedbacks
Content-Type: application/json
Authorization: Bearer a661d09d928cec6bafef294bc8c9a699392cac2be2e98981da79c1bf41b0e5ed
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
      "user_id": 854,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:06.270Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 853,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:06.260Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/124/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a661d09d928cec6bafef294bc8c9a699392cac2be2e98981da79c1bf41b0e5ed"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 7d8825229a1835a4bf3fe4e5756f25c7cd724ab07099f906059ca54e55812a5f
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 494,
      "chapter_id": 91,
      "position": 40,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:33.887Z",
      "created_at": "2016-11-16T17:23:33.770Z",
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
      "id": 46,
      "obfuscated_id": "urkHiAaH08E",
      "author_id": 485,
      "chapter_id": 88,
      "position": 37,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:33.081Z",
      "created_at": "2016-11-16T17:23:32.965Z",
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
          "id": 95,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 96,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 488,
      "chapter_id": 89,
      "position": 38,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:33.348Z",
      "created_at": "2016-11-16T17:23:33.235Z",
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
      "id": 48,
      "obfuscated_id": "oqXJ8Hi_AE4",
      "author_id": 491,
      "chapter_id": 90,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:33.615Z",
      "created_at": "2016-11-16T17:23:33.501Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 497,
      "chapter_id": 92,
      "position": 41,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:34.154Z",
      "created_at": "2016-11-16T17:23:34.044Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d8825229a1835a4bf3fe4e5756f25c7cd724ab07099f906059ca54e55812a5f"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 07e0fa12c05560e5097ea8af9379ea71774e918c1532893576e4e8e168a347a1
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 481,
      "chapter_id": 87,
      "position": 36,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:32.755Z",
      "created_at": "2016-11-16T17:23:32.642Z",
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
          "id": 93,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 94,
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
	-H "Authorization: Bearer 07e0fa12c05560e5097ea8af9379ea71774e918c1532893576e4e8e168a347a1"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/57/republish
Content-Type: application/json
Authorization: Bearer f755d3fa9c72e605a4c85737dc8693ee57b8c07191d9f7821e8e348d0b0b87a0
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/57/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f755d3fa9c72e605a4c85737dc8693ee57b8c07191d9f7821e8e348d0b0b87a0"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 31b6763b4d21fd7aac56d8bed690a4457b0d7cdd01fb6a942807198ece541aa2
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":134,"published":false}}
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
    "creator_id": 328,
    "id": 132,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 116,
    "additional_university_ids": [

    ],
    "discipline_id": 135,
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
    "updated_at": "2016-11-16T17:23:21.050Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 134,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":134,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31b6763b4d21fd7aac56d8bed690a4457b0d7cdd01fb6a942807198ece541aa2"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d47a4be5a7371d7dc66aaf1b2c317a637d6a71ec78ba0f31dd9a23475c496b03
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
      "creator_id": 311,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "discipline_id": 120,
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
      "updated_at": "2016-11-16T17:23:19.201Z",
      "shortname": "fu-course-103",
      "topic_id": 119,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 311,
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-104",
      "html_url": "https://goskive.com/course/fu-course-104",
      "slug": "fu-course-104",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "discipline_id": 121,
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
      "updated_at": "2016-11-16T17:23:19.242Z",
      "shortname": "fu-course-104",
      "topic_id": 120,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 312,
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "discipline_id": 122,
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
      "updated_at": "2016-11-16T17:23:19.288Z",
      "shortname": "fu-course-105",
      "topic_id": 121,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 312,
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "discipline_id": 123,
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
      "chapters_updated_at": "2016-11-16T17:23:19.146Z",
      "updated_at": "2016-11-16T17:23:19.624Z",
      "shortname": "fu-course-106",
      "topic_id": 122,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d47a4be5a7371d7dc66aaf1b2c317a637d6a71ec78ba0f31dd9a23475c496b03"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d8f531445d826d83f080aea2180be7b8f25b5d26c77ebcf0ecf36b5cabd6c34a
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
      "creator_id": 317,
      "id": 121,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 109,
      "additional_university_ids": [

      ],
      "discipline_id": 124,
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
      "updated_at": "2016-11-16T17:23:19.761Z",
      "shortname": "fu-course-107",
      "topic_id": 123,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 317,
      "id": 122,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 109,
      "additional_university_ids": [

      ],
      "discipline_id": 125,
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
      "updated_at": "2016-11-16T17:23:19.798Z",
      "shortname": "fu-course-108",
      "topic_id": 124,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 318,
      "id": 123,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 109,
      "additional_university_ids": [

      ],
      "discipline_id": 126,
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
      "updated_at": "2016-11-16T17:23:19.842Z",
      "shortname": "fu-course-109",
      "topic_id": 125,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 318,
      "id": 124,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 109,
      "additional_university_ids": [

      ],
      "discipline_id": 127,
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
      "updated_at": "2016-11-16T17:23:19.880Z",
      "shortname": "fu-course-110",
      "topic_id": 126,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8f531445d826d83f080aea2180be7b8f25b5d26c77ebcf0ecf36b5cabd6c34a"
```
