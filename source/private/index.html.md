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
DELETE /v2/chapters/151
Content-Type: application/json
Authorization: Bearer d4c26ab55f8b50ad9459f70704cffcbaa85aa407f4297c49e8134b1e4fbb32f2
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/151" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4c26ab55f8b50ad9459f70704cffcbaa85aa407f4297c49e8134b1e4fbb32f2"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/154
Content-Type: application/json
Authorization: Bearer 80af693804ee6ee032e4614c4fe88f25ce002d22587765d6eae7e4a19dc46151
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
    "id": 154,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-11T17:00:27.330Z",
    "course_id": 269,
    "author_id": 821,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-11T17:00:26.773Z",
    "questions_updated_at": "2016-10-11T17:00:26.773Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 824,
        "chapter_id": 154,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:27.272Z",
        "created_at": "2016-10-11T17:00:27.272Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 825,
        "chapter_id": 154,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:27.312Z",
        "created_at": "2016-10-11T17:00:27.312Z",
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
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 822,
        "chapter_id": 154,
        "position": 102,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:27.000Z",
        "created_at": "2016-10-11T17:00:26.890Z",
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
      },
      {
        "id": 116,
        "obfuscated_id": "PhHGVKqnHFA",
        "author_id": 823,
        "chapter_id": 154,
        "position": 103,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:27.198Z",
        "created_at": "2016-10-11T17:00:27.076Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/154" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80af693804ee6ee032e4614c4fe88f25ce002d22587765d6eae7e4a19dc46151"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/157
Content-Type: application/json
Authorization: Bearer 721e5ba1cd1dfe98e9a3abb10de85c89cf0b98fe5e45bdee4c63c5025e148a77
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
    "id": 157,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-11T17:00:28.442Z",
    "course_id": 272,
    "author_id": 837,
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
curl "api.goskive.com/v2/chapters/157" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 721e5ba1cd1dfe98e9a3abb10de85c89cf0b98fe5e45bdee4c63c5025e148a77"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer 2a2aae1c44ac51851ce5cccd61ad8665b33eb986eb1e92dabe6c74dde3489d46
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
	-H "Authorization: Bearer 2a2aae1c44ac51851ce5cccd61ad8665b33eb986eb1e92dabe6c74dde3489d46"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 065b859d1da72ce9d2f43c9d79814f13a02b408a7e8610df5133345584a15dc6
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
      "author_id": 493,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:00.176Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 495,
      "reply_to_id": 32,
      "created_at": "2016-10-11T17:00:00.270Z",
      "status": "published",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 497,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:00.368Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 499,
      "reply_to_id": 34,
      "created_at": "2016-10-11T17:00:00.487Z",
      "status": "published",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 501,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:00.603Z",
      "status": "reported",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 503,
      "reply_to_id": 36,
      "created_at": "2016-10-11T17:00:00.750Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 505,
      "reply_to_id": 36,
      "created_at": "2016-10-11T17:00:00.840Z",
      "status": "published",
      "subject_id": 154,
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
	-H "Authorization: Bearer 065b859d1da72ce9d2f43c9d79814f13a02b408a7e8610df5133345584a15dc6"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d6c581fe4bfee401302d71fcdd1bbbe1121d57f25a78588a719cb58d6f47deee
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
      "id": 39,
      "author_id": 508,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:00.992Z",
      "status": "published",
      "subject_id": 155,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 510,
      "reply_to_id": 39,
      "created_at": "2016-10-11T17:00:01.082Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 512,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:01.173Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 514,
      "reply_to_id": 41,
      "created_at": "2016-10-11T17:00:01.261Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 516,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:01.357Z",
      "status": "reported",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 518,
      "reply_to_id": 43,
      "created_at": "2016-10-11T17:00:01.451Z",
      "status": "published",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 520,
      "reply_to_id": 43,
      "created_at": "2016-10-11T17:00:01.546Z",
      "status": "published",
      "subject_id": 161,
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
	-H "Authorization: Bearer d6c581fe4bfee401302d71fcdd1bbbe1121d57f25a78588a719cb58d6f47deee"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 365333ed328d3d514300e8bf500a190ff10bcba6776a2028dc57e596cfabc194
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
      "id": 19,
      "author_id": 465,
      "reply_to_id": 18,
      "created_at": "2016-10-11T16:59:58.885Z",
      "status": "published",
      "subject_id": 135,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 469,
      "reply_to_id": 20,
      "created_at": "2016-10-11T16:59:59.070Z",
      "status": "published",
      "subject_id": 137,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 473,
      "reply_to_id": 22,
      "created_at": "2016-10-11T16:59:59.252Z",
      "status": "published",
      "subject_id": 139,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 475,
      "reply_to_id": 22,
      "created_at": "2016-10-11T16:59:59.344Z",
      "status": "published",
      "subject_id": 140,
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
	-H "Authorization: Bearer 365333ed328d3d514300e8bf500a190ff10bcba6776a2028dc57e596cfabc194"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 0edcad694e49916466e38ef6840f4ee9228f5acb1748f9a4c1fe8978b98d6424
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
      "id": 29,
      "author_id": 486,
      "reply_to_id": null,
      "created_at": "2016-10-11T16:59:59.855Z",
      "status": "reported",
      "subject_id": 145,
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
	-H "Authorization: Bearer 0edcad694e49916466e38ef6840f4ee9228f5acb1748f9a4c1fe8978b98d6424"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/16/republish
Content-Type: application/json
Authorization: Bearer 9be4fe7dfd3f0e6f7f7e20ea3194e49efe95721066c9e8c3200ed68038af7b1a
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9be4fe7dfd3f0e6f7f7e20ea3194e49efe95721066c9e8c3200ed68038af7b1a"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f1223414b2826bf97a03d438d90c51425d7bc67aa0dfe4cfce1fa812ebd4a69d
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
    "id": 182,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-11T17:00:32.537Z",
    "course_id": 292,
    "author_id": 910,
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
	-H "Authorization: Bearer f1223414b2826bf97a03d438d90c51425d7bc67aa0dfe4cfce1fa812ebd4a69d"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/293/chapters
Content-Type: application/json
Authorization: Bearer 2c2ca4dfeedca343fc7d89676b28d930fa9729032cbc7c5bad054e88162c729f
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
    "id": 183,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-11T17:00:32.677Z",
    "course_id": 293,
    "author_id": 912,
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
curl "api.goskive.com/v2/courses/293/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c2ca4dfeedca343fc7d89676b28d930fa9729032cbc7c5bad054e88162c729f"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fc80d96ff32d7f85830990af303ec5fad96cc0838edfad44674af11caac58c0e
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
      "id": 163,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-11T17:00:29.972Z",
      "course_id": 281,
      "author_id": 867,
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
      "id": 164,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-11T17:00:29.997Z",
      "course_id": 281,
      "author_id": 868,
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
      "id": 165,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-11T17:00:30.255Z",
      "course_id": 281,
      "author_id": 869,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-11T17:00:29.893Z",
      "questions_updated_at": "2016-10-11T17:00:29.893Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc80d96ff32d7f85830990af303ec5fad96cc0838edfad44674af11caac58c0e"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 754dc03da607af97bfc895d3660b8337dccc2734a50a9c7b8409d25700a26c84
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
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-11T17:00:30.409Z",
      "course_id": 282,
      "author_id": 874,
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
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-11T17:00:30.436Z",
      "course_id": 282,
      "author_id": 875,
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
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-11T17:00:30.462Z",
      "course_id": 282,
      "author_id": 876,
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
	-H "Authorization: Bearer 754dc03da607af97bfc895d3660b8337dccc2734a50a9c7b8409d25700a26c84"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/11
Content-Type: application/json
Authorization: Bearer 81e2ac8efb6ea8c8ed973977c998593d55894e6869c93c44859b0f31a47be67a
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81e2ac8efb6ea8c8ed973977c998593d55894e6869c93c44859b0f31a47be67a"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 535820a32a0089be6f5f3a35b602685d212bf143d3cdcf09a42d5c8b035c7fa1
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
	-H "Authorization: Bearer 535820a32a0089be6f5f3a35b602685d212bf143d3cdcf09a42d5c8b035c7fa1"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer de84d5fa6971f4462caa64138b9a297f1b8fcab0b7f1a3e7f6aee0886fd8677e
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
    "creator_id": 3,
    "id": 2,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 2,
    "additional_university_ids": [

    ],
    "topic_id": 4,
    "discipline_id": 5,
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
    "chapters_updated_at": "2016-10-11T16:59:14.187Z",
    "updated_at": "2016-10-11T16:59:15.789Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 1,
        "title": "Clever Chapter Title 1",
        "position": 1,
        "updated_at": "2016-10-11T16:59:15.740Z",
        "course_id": 2,
        "author_id": 3,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-11T16:59:14.187Z",
        "questions_updated_at": "2016-10-11T16:59:14.187Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 2,
        "title": "Clever Chapter Title 2",
        "position": 2,
        "updated_at": "2016-10-11T16:59:15.782Z",
        "course_id": 2,
        "author_id": 3,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-11T16:59:14.187Z",
        "questions_updated_at": "2016-10-11T16:59:14.187Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 3,
        "chapter_id": 1,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.576Z",
        "created_at": "2016-10-11T16:59:15.576Z",
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
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 3,
        "chapter_id": 2,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.650Z",
        "created_at": "2016-10-11T16:59:15.650Z",
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
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 3,
        "chapter_id": 1,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.619Z",
        "created_at": "2016-10-11T16:59:15.619Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 3,
        "chapter_id": 2,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.690Z",
        "created_at": "2016-10-11T16:59:15.690Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 6,
        "chapter_id": 1,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.730Z",
        "created_at": "2016-10-11T16:59:15.730Z",
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
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 7,
        "chapter_id": 2,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:15.771Z",
        "created_at": "2016-10-11T16:59:15.771Z",
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
	-H "Authorization: Bearer de84d5fa6971f4462caa64138b9a297f1b8fcab0b7f1a3e7f6aee0886fd8677e"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/10
Content-Type: application/json
Authorization: Bearer 07cf029c5dcaf7505844b35d2d6576300698ab974481a1ac74da0e178b7a1e27
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
    "creator_id": 33,
    "id": 10,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 10,
    "additional_university_ids": [

    ],
    "topic_id": 12,
    "discipline_id": 13,
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
    "updated_at": "2016-10-11T16:59:21.439Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/10" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07cf029c5dcaf7505844b35d2d6576300698ab974481a1ac74da0e178b7a1e27"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1af5e87ccc8cd8b7d46098574d2f11d2e362f7e645a367d6e02f6e675f06720f
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
    "creator_id": 29,
    "id": 8,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 8,
    "additional_university_ids": [

    ],
    "topic_id": 10,
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
    "published": false,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-10-11T16:59:21.177Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1af5e87ccc8cd8b7d46098574d2f11d2e362f7e645a367d6e02f6e675f06720f"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer e0b7a7f66431097b711b4e57dfd3885dd63337010fa7549fd93d148838824d48
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
      "id": 32,
      "user_id": 620,
      "feedbackable_id": 80,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T17:00:08.162Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 624,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T17:00:08.478Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 628,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T17:00:08.794Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 632,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T17:00:09.109Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 636,
      "feedbackable_id": 84,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-11T17:00:09.427Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0b7a7f66431097b711b4e57dfd3885dd63337010fa7549fd93d148838824d48"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 28de327e3f319500be4e35fabb17e7f8ec27215f7eab5547f69275517cc43768
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
      "id": 31,
      "user_id": 615,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-11T17:00:07.779Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28de327e3f319500be4e35fabb17e7f8ec27215f7eab5547f69275517cc43768"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer f4c9bd7e4bcfcf1a828b251d99ae13b03804690ce696ccb1eaa2819d25a6d7d4
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
curl "api.goskive.com/v2/files/4" -d '' -X DELETE \
	-H "Authorization: Bearer f4c9bd7e4bcfcf1a828b251d99ae13b03804690ce696ccb1eaa2819d25a6d7d4" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/63/feedbacks
Content-Type: application/json
Authorization: Bearer c8dcfcef2a89ac180aefc86315aa3987e08d69f75ccaa13b310a389f310d8e98
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
      "id": 17,
      "user_id": 319,
      "feedbackable_id": 63,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:45.487Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 318,
      "feedbackable_id": 63,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:45.475Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/63/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8dcfcef2a89ac180aefc86315aa3987e08d69f75ccaa13b310a389f310d8e98"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 968ae9bf8a9b00879aca0dfe149281d56aacc3b1aec7f5033ad17c2054fb4716
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 115,
      "chapter_id": 28,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:29.293Z",
      "created_at": "2016-10-11T16:59:29.293Z",
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 118,
      "chapter_id": 29,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:29.440Z",
      "created_at": "2016-10-11T16:59:29.440Z",
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
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 121,
      "chapter_id": 30,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:29.593Z",
      "created_at": "2016-10-11T16:59:29.593Z",
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 124,
      "chapter_id": 31,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:29.740Z",
      "created_at": "2016-10-11T16:59:29.740Z",
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
      "author_id": 127,
      "chapter_id": 32,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:29.883Z",
      "created_at": "2016-10-11T16:59:29.883Z",
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
	-H "Authorization: Bearer 968ae9bf8a9b00879aca0dfe149281d56aacc3b1aec7f5033ad17c2054fb4716"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 89229dd933c46bb5510b5d36cb534841bc65344d9911b2833b163152f8dc7ff5
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
      "author_id": 95,
      "chapter_id": 22,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:28.260Z",
      "created_at": "2016-10-11T16:59:28.260Z",
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
	-H "Authorization: Bearer 89229dd933c46bb5510b5d36cb534841bc65344d9911b2833b163152f8dc7ff5"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/28/republish
Content-Type: application/json
Authorization: Bearer 8706eea4e502eb80b774c8b1221ddde80af080f9433756f291f79a5c5b8fb059
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8706eea4e502eb80b774c8b1221ddde80af080f9433756f291f79a5c5b8fb059"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/45/feedbacks
Content-Type: application/json
Authorization: Bearer 6316b79844c1d9e6963eec8cad7fcb9f58e4338123345d97a4047f25068761b3
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
      "id": 9,
      "user_id": 280,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:43.285Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 279,
      "feedbackable_id": 45,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:43.272Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/45/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6316b79844c1d9e6963eec8cad7fcb9f58e4338123345d97a4047f25068761b3"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 2b33df452aca03e6d908350954720aa22f77624a9ebd56011d8714274ca0dd6f
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 358,
      "chapter_id": 81,
      "position": 55,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:49.568Z",
      "created_at": "2016-10-11T16:59:49.446Z",
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
    },
    {
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 349,
      "chapter_id": 78,
      "position": 52,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:48.689Z",
      "created_at": "2016-10-11T16:59:48.573Z",
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
          "id": 109,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 110,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 352,
      "chapter_id": 79,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:48.982Z",
      "created_at": "2016-10-11T16:59:48.863Z",
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
          "id": 111,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 112,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 355,
      "chapter_id": 80,
      "position": 54,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:49.270Z",
      "created_at": "2016-10-11T16:59:49.151Z",
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
          "id": 113,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 114,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 361,
      "chapter_id": 82,
      "position": 56,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:49.864Z",
      "created_at": "2016-10-11T16:59:49.747Z",
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
          "id": 117,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 118,
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
	-H "Authorization: Bearer 2b33df452aca03e6d908350954720aa22f77624a9ebd56011d8714274ca0dd6f"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 87cdb2c5fa143c2578f766e1590d481ef4d2a68f5bd22b61da9b56d9a83b5bd9
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 377,
      "chapter_id": 87,
      "position": 61,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T16:59:51.403Z",
      "created_at": "2016-10-11T16:59:51.289Z",
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
          "id": 127,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 128,
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
	-H "Authorization: Bearer 87cdb2c5fa143c2578f766e1590d481ef4d2a68f5bd22b61da9b56d9a83b5bd9"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/70/republish
Content-Type: application/json
Authorization: Bearer 1d37ee41219e29856157af5f27cff3cc701d8cd1cd9fdcc427d660fe783c6281
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/70/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d37ee41219e29856157af5f27cff3cc701d8cd1cd9fdcc427d660fe783c6281"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 12b5a5c57de16685841576fc6efb3764fa7f2a07da4d4750c052886a7f87570b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":257,"published":false}}
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
    "creator_id": 750,
    "id": 245,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 230,
    "additional_university_ids": [

    ],
    "topic_id": 257,
    "discipline_id": 258,
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
    "updated_at": "2016-10-11T17:00:19.192Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":257,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12b5a5c57de16685841576fc6efb3764fa7f2a07da4d4750c052886a7f87570b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 82334dfe0736accd3e2815a4f2777dbbcc163ddf5f20b44ebb9dea082ab9552b
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
      "creator_id": 723,
      "id": 221,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 221,
      "additional_university_ids": [

      ],
      "topic_id": 233,
      "discipline_id": 234,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
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
      "updated_at": "2016-10-11T17:00:16.493Z",
      "shortname": "fu-course-192"
    },
    {
      "creator_id": 723,
      "id": 222,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-193",
      "html_url": "https://goskive.com/course/fu-course-193",
      "slug": "fu-course-193",
      "university_id": 221,
      "additional_university_ids": [

      ],
      "topic_id": 234,
      "discipline_id": 235,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 193",
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
      "updated_at": "2016-10-11T17:00:16.535Z",
      "shortname": "fu-course-193"
    },
    {
      "creator_id": 724,
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-194",
      "html_url": "https://goskive.com/course/fu-course-194",
      "slug": "fu-course-194",
      "university_id": 221,
      "additional_university_ids": [

      ],
      "topic_id": 235,
      "discipline_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 194",
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
      "updated_at": "2016-10-11T17:00:16.585Z",
      "shortname": "fu-course-194"
    },
    {
      "creator_id": 724,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 221,
      "additional_university_ids": [

      ],
      "topic_id": 236,
      "discipline_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
      "chapters_updated_at": "2016-10-11T17:00:16.889Z",
      "updated_at": "2016-10-11T17:00:16.896Z",
      "shortname": "fu-course-195"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82334dfe0736accd3e2815a4f2777dbbcc163ddf5f20b44ebb9dea082ab9552b"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a1a0e90ce9ef5c20aef566e2381b9cfd98fff1015110cfb21e60aeaefa731733
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
      "creator_id": 729,
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 222,
      "additional_university_ids": [

      ],
      "topic_id": 237,
      "discipline_id": 238,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
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
      "updated_at": "2016-10-11T17:00:17.058Z",
      "shortname": "fu-course-196"
    },
    {
      "creator_id": 729,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-197",
      "html_url": "https://goskive.com/course/fu-course-197",
      "slug": "fu-course-197",
      "university_id": 222,
      "additional_university_ids": [

      ],
      "topic_id": 238,
      "discipline_id": 239,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 197",
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
      "updated_at": "2016-10-11T17:00:17.103Z",
      "shortname": "fu-course-197"
    },
    {
      "creator_id": 730,
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-198",
      "html_url": "https://goskive.com/course/fu-course-198",
      "slug": "fu-course-198",
      "university_id": 222,
      "additional_university_ids": [

      ],
      "topic_id": 239,
      "discipline_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 198",
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
      "updated_at": "2016-10-11T17:00:17.155Z",
      "shortname": "fu-course-198"
    },
    {
      "creator_id": 730,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 222,
      "additional_university_ids": [

      ],
      "topic_id": 240,
      "discipline_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
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
      "updated_at": "2016-10-11T17:00:17.198Z",
      "shortname": "fu-course-199"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1a0e90ce9ef5c20aef566e2381b9cfd98fff1015110cfb21e60aeaefa731733"
```
