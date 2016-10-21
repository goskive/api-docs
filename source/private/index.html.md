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
DELETE /v2/chapters/38
Content-Type: application/json
Authorization: Bearer afc6dc7a9c63b60572c1ad36c7e60bf9f4c02f347ad595730184eb226746dc62
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/38" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afc6dc7a9c63b60572c1ad36c7e60bf9f4c02f347ad595730184eb226746dc62"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/32
Content-Type: application/json
Authorization: Bearer a2a3d7214ee910d6b1b3a37a2044a851122f9158bb678dde07b217aa2ff01721
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
    "id": 32,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-21T15:03:54.462Z",
    "course_id": 80,
    "author_id": 167,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-21T15:03:53.898Z",
    "questions_updated_at": "2016-10-21T15:03:53.898Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 170,
        "chapter_id": 32,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:54.381Z",
        "created_at": "2016-10-21T15:03:54.381Z",
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
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 171,
        "chapter_id": 32,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:54.420Z",
        "created_at": "2016-10-21T15:03:54.420Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 168,
        "chapter_id": 32,
        "position": 47,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:54.118Z",
        "created_at": "2016-10-21T15:03:54.007Z",
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
      },
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 169,
        "chapter_id": 32,
        "position": 48,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:54.310Z",
        "created_at": "2016-10-21T15:03:54.190Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/32" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2a3d7214ee910d6b1b3a37a2044a851122f9158bb678dde07b217aa2ff01721"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/36
Content-Type: application/json
Authorization: Bearer 63f1ff437db94a1bccc5346e09c022b056d7c012081f5053aefb8b8a2c4d8ded
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
    "id": 36,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-21T15:03:55.613Z",
    "course_id": 84,
    "author_id": 186,
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
curl "api.goskive.com/v2/chapters/36" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63f1ff437db94a1bccc5346e09c022b056d7c012081f5053aefb8b8a2c4d8ded"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/43
Content-Type: application/json
Authorization: Bearer b8e4d96c660faf8e00bfd4ab29c2e31a799b1a1ba115ed9b2e03d6de7c6a8b1d
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
	-H "Authorization: Bearer b8e4d96c660faf8e00bfd4ab29c2e31a799b1a1ba115ed9b2e03d6de7c6a8b1d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5081b1012676bf1d17cb0a1116307d77e833dd16fba2cb0924198d983ea62c0e
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
      "id": 8,
      "author_id": 675,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:32.973Z",
      "status": "published",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 677,
      "reply_to_id": 8,
      "created_at": "2016-10-21T15:04:33.064Z",
      "status": "published",
      "subject_id": 220,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 679,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:33.157Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 681,
      "reply_to_id": 10,
      "created_at": "2016-10-21T15:04:33.245Z",
      "status": "published",
      "subject_id": 222,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 683,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:33.334Z",
      "status": "reported",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 685,
      "reply_to_id": 12,
      "created_at": "2016-10-21T15:04:33.424Z",
      "status": "published",
      "subject_id": 224,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 687,
      "reply_to_id": 12,
      "created_at": "2016-10-21T15:04:33.514Z",
      "status": "published",
      "subject_id": 225,
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
	-H "Authorization: Bearer 5081b1012676bf1d17cb0a1116307d77e833dd16fba2cb0924198d983ea62c0e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2a0b74316a4ef3fcbecd19ded2ade72757666218ecc36aab63403219093de62e
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
      "id": 15,
      "author_id": 690,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:33.670Z",
      "status": "published",
      "subject_id": 226,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 692,
      "reply_to_id": 15,
      "created_at": "2016-10-21T15:04:33.760Z",
      "status": "published",
      "subject_id": 227,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 694,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:33.851Z",
      "status": "published",
      "subject_id": 228,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 696,
      "reply_to_id": 17,
      "created_at": "2016-10-21T15:04:33.942Z",
      "status": "published",
      "subject_id": 229,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 698,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:34.035Z",
      "status": "reported",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 700,
      "reply_to_id": 19,
      "created_at": "2016-10-21T15:04:34.126Z",
      "status": "published",
      "subject_id": 231,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 702,
      "reply_to_id": 19,
      "created_at": "2016-10-21T15:04:34.231Z",
      "status": "published",
      "subject_id": 232,
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
	-H "Authorization: Bearer 2a0b74316a4ef3fcbecd19ded2ade72757666218ecc36aab63403219093de62e"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer dd6f12545281a95c0bcc77cf7561ebea99a509c231a18c05865c309cc4d688d6
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
      "id": 23,
      "author_id": 707,
      "reply_to_id": 22,
      "created_at": "2016-10-21T15:04:34.971Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 711,
      "reply_to_id": 24,
      "created_at": "2016-10-21T15:04:35.170Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 715,
      "reply_to_id": 26,
      "created_at": "2016-10-21T15:04:35.357Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 717,
      "reply_to_id": 26,
      "created_at": "2016-10-21T15:04:35.477Z",
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
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd6f12545281a95c0bcc77cf7561ebea99a509c231a18c05865c309cc4d688d6"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer d6bf45bd96dee89c9156440b50e5ae63c5a963cae3e0743d4cf5b22b996c5607
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
      "id": 40,
      "author_id": 743,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:36.643Z",
      "status": "reported",
      "subject_id": 251,
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
	-H "Authorization: Bearer d6bf45bd96dee89c9156440b50e5ae63c5a963cae3e0743d4cf5b22b996c5607"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/48/republish
Content-Type: application/json
Authorization: Bearer d79482a8e7030044fa6f8d0ddf9ffb8d4816ab8095e1fea5eaaece590d326335
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/48/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d79482a8e7030044fa6f8d0ddf9ffb8d4816ab8095e1fea5eaaece590d326335"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e45337236428ae156be65b2381dd599c877efb9beaabba722f1d834b1a00ec79
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
    "updated_at": "2016-10-21T15:04:26.400Z",
    "course_id": 187,
    "author_id": 564,
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
	-H "Authorization: Bearer e45337236428ae156be65b2381dd599c877efb9beaabba722f1d834b1a00ec79"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/189/chapters
Content-Type: application/json
Authorization: Bearer ac6e2e3a7844eff9fe03bd7b69d3f0e275ffe85a5fde2ed3c2986188ef415b05
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
    "updated_at": "2016-10-21T15:04:26.647Z",
    "course_id": 189,
    "author_id": 568,
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
curl "api.goskive.com/v2/courses/189/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac6e2e3a7844eff9fe03bd7b69d3f0e275ffe85a5fde2ed3c2986188ef415b05"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d0a5b2be63ce49b68b0bebf94f378c27616ab95663204ad1f8ebc1cc255be063
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
      "id": 121,
      "title": "Clever Chapter Title 109",
      "position": 1,
      "updated_at": "2016-10-21T15:04:25.135Z",
      "course_id": 181,
      "author_id": 541,
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
      "id": 122,
      "title": "Clever Chapter Title 110",
      "position": 2,
      "updated_at": "2016-10-21T15:04:25.160Z",
      "course_id": 181,
      "author_id": 542,
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
      "id": 123,
      "title": "Clever Chapter Title 111",
      "position": 3,
      "updated_at": "2016-10-21T15:04:25.419Z",
      "course_id": 181,
      "author_id": 543,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-21T15:04:25.057Z",
      "questions_updated_at": "2016-10-21T15:04:25.057Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0a5b2be63ce49b68b0bebf94f378c27616ab95663204ad1f8ebc1cc255be063"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 46debb2e13b791e33bb13154b522cafdb467269f7fc39cce085be406385ac1c9
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
      "id": 124,
      "title": "Clever Chapter Title 112",
      "position": 1,
      "updated_at": "2016-10-21T15:04:25.706Z",
      "course_id": 183,
      "author_id": 550,
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
      "id": 125,
      "title": "Clever Chapter Title 113",
      "position": 2,
      "updated_at": "2016-10-21T15:04:25.732Z",
      "course_id": 183,
      "author_id": 551,
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
      "id": 126,
      "title": "Clever Chapter Title 114",
      "position": 3,
      "updated_at": "2016-10-21T15:04:25.757Z",
      "course_id": 183,
      "author_id": 552,
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
	-H "Authorization: Bearer 46debb2e13b791e33bb13154b522cafdb467269f7fc39cce085be406385ac1c9"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/28
Content-Type: application/json
Authorization: Bearer 005999e75b26490c02a783e6e136c602040e79636f53a4c11d90b4fc840f4c1f
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/28" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 005999e75b26490c02a783e6e136c602040e79636f53a4c11d90b4fc840f4c1f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer aa45115a21ea14ad25d80c20d0db432cf5c36c045189667b3347ffa52761b6c7
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
	-H "Authorization: Bearer aa45115a21ea14ad25d80c20d0db432cf5c36c045189667b3347ffa52761b6c7"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer e00a373e8a3b66db203bf8566055a2ad5992e61c9a6cba280aacc8858fdb9061
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
    "creator_id": 78,
    "id": 26,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 26,
    "additional_university_ids": [

    ],
    "topic_id": 26,
    "discipline_id": 26,
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
    "chapters_updated_at": "2016-10-21T15:03:43.916Z",
    "updated_at": "2016-10-21T15:03:45.364Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 14,
        "title": "Clever Chapter Title 14",
        "position": 1,
        "updated_at": "2016-10-21T15:03:45.318Z",
        "course_id": 26,
        "author_id": 78,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-21T15:03:43.916Z",
        "questions_updated_at": "2016-10-21T15:03:43.916Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 15,
        "title": "Clever Chapter Title 15",
        "position": 2,
        "updated_at": "2016-10-21T15:03:45.357Z",
        "course_id": 26,
        "author_id": 78,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-21T15:03:43.916Z",
        "questions_updated_at": "2016-10-21T15:03:43.916Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 78,
        "chapter_id": 14,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.159Z",
        "created_at": "2016-10-21T15:03:45.159Z",
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
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 78,
        "chapter_id": 15,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.228Z",
        "created_at": "2016-10-21T15:03:45.228Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 78,
        "chapter_id": 14,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.198Z",
        "created_at": "2016-10-21T15:03:45.198Z",
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
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 78,
        "chapter_id": 15,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.268Z",
        "created_at": "2016-10-21T15:03:45.268Z",
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
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 81,
        "chapter_id": 14,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.308Z",
        "created_at": "2016-10-21T15:03:45.308Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 82,
        "chapter_id": 15,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.346Z",
        "created_at": "2016-10-21T15:03:45.346Z",
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
	-H "Authorization: Bearer e00a373e8a3b66db203bf8566055a2ad5992e61c9a6cba280aacc8858fdb9061"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/20
Content-Type: application/json
Authorization: Bearer fa5a4022c916bf42e09d1dbf6bf3eb1e663f954397c188677f35723f1491cd29
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
    "creator_id": 60,
    "id": 20,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 20,
    "additional_university_ids": [

    ],
    "topic_id": 20,
    "discipline_id": 20,
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
    "updated_at": "2016-10-21T15:03:40.405Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/20" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa5a4022c916bf42e09d1dbf6bf3eb1e663f954397c188677f35723f1491cd29"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 42a3b7f8504fe343228803c94af582a536c8ff8c408207458d2e3e8d8dfe8b32
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
    "creator_id": 63,
    "id": 22,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 22,
    "additional_university_ids": [

    ],
    "topic_id": 22,
    "discipline_id": 22,
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
    "updated_at": "2016-10-21T15:03:40.694Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42a3b7f8504fe343228803c94af582a536c8ff8c408207458d2e3e8d8dfe8b32"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 8fe3f7dd5976a12b70fcf501fb33a0407cde4902755651bf9f6cf3583e0fb5c6
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
      "id": 16,
      "user_id": 383,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:13.517Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 387,
      "feedbackable_id": 96,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:13.822Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 391,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:14.135Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 395,
      "feedbackable_id": 98,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:14.441Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 20,
      "user_id": 399,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-21T15:04:14.756Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fe3f7dd5976a12b70fcf501fb33a0407cde4902755651bf9f6cf3583e0fb5c6"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer accefbca1696b9ce62d29ef0111634609fe1ad80bee7efab450387f084526311
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
      "id": 6,
      "user_id": 341,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-21T15:04:10.330Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer accefbca1696b9ce62d29ef0111634609fe1ad80bee7efab450387f084526311"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/3
Content-Type: application/json
Authorization: Bearer fa281a57aa4e0bb82fc311105ad3b775233fe0f4d8d5a6ab0494a5ec1b784a24
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa281a57aa4e0bb82fc311105ad3b775233fe0f4d8d5a6ab0494a5ec1b784a24"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 0494db43e1226240f8be18abb02e1fc603746f8069b2e746cb86afe18d2189d1
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
      "id": 780,
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
      "created_at": "2016-10-21T15:04:38.560Z",
      "updated_at": "2016-10-21T15:04:38.560Z"
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
    "created_at": "2016-10-21T15:04:38.640Z",
    "updated_at": "2016-10-21T15:04:38.640Z",
    "course_id": 265,
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
	-H "Authorization: Bearer 0494db43e1226240f8be18abb02e1fc603746f8069b2e746cb86afe18d2189d1"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/86/feedbacks
Content-Type: application/json
Authorization: Bearer f74fc813c2db40d036cbc660d842a885d748bc2c0c1e27e30ae8c5d9b2704f14
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
      "id": 45,
      "user_id": 844,
      "feedbackable_id": 86,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:43.760Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 843,
      "feedbackable_id": 86,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:43.748Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/86/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f74fc813c2db40d036cbc660d842a885d748bc2c0c1e27e30ae8c5d9b2704f14"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 4c87b23b37c42c01151470df5a59ab9e3a5b58822a50d41c532585456ade9367
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 585,
      "chapter_id": 134,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:27.634Z",
      "created_at": "2016-10-21T15:04:27.634Z",
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
      "author_id": 588,
      "chapter_id": 135,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:27.773Z",
      "created_at": "2016-10-21T15:04:27.773Z",
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
      "author_id": 591,
      "chapter_id": 136,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:27.913Z",
      "created_at": "2016-10-21T15:04:27.913Z",
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
      "author_id": 594,
      "chapter_id": 137,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:28.054Z",
      "created_at": "2016-10-21T15:04:28.054Z",
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
      "author_id": 597,
      "chapter_id": 138,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:28.195Z",
      "created_at": "2016-10-21T15:04:28.195Z",
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
	-H "Authorization: Bearer 4c87b23b37c42c01151470df5a59ab9e3a5b58822a50d41c532585456ade9367"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer c9f8f62cc360483227c13e8778f4a7c3e7a9a84c7795cc81df203f637139328f
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 629,
      "chapter_id": 148,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:29.730Z",
      "created_at": "2016-10-21T15:04:29.730Z",
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
	-H "Authorization: Bearer c9f8f62cc360483227c13e8778f4a7c3e7a9a84c7795cc81df203f637139328f"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/72/republish
Content-Type: application/json
Authorization: Bearer 5e3e634feef12533246522c4f4d7858466b33381844a5293d7bb5c683140e2b3
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e3e634feef12533246522c4f4d7858466b33381844a5293d7bb5c683140e2b3"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/105/feedbacks
Content-Type: application/json
Authorization: Bearer 62e9bdaf32981842e17027b4172f2ee6519f8798040f3ecdfc0d1d2e74191514
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
      "id": 35,
      "user_id": 490,
      "feedbackable_id": 105,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:21.194Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 489,
      "feedbackable_id": 105,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:21.183Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/105/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62e9bdaf32981842e17027b4172f2ee6519f8798040f3ecdfc0d1d2e74191514"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer e69c4f61cfe287df14d8c24398b1e0b9314f9b4340207c199a4cffa4e4be4e98
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
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 236,
      "chapter_id": 44,
      "position": 56,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:03:59.588Z",
      "created_at": "2016-10-21T15:03:59.469Z",
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
      "author_id": 239,
      "chapter_id": 45,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:03:59.870Z",
      "created_at": "2016-10-21T15:03:59.752Z",
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 242,
      "chapter_id": 46,
      "position": 58,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:00.164Z",
      "created_at": "2016-10-21T15:04:00.040Z",
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 245,
      "chapter_id": 47,
      "position": 59,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:00.461Z",
      "created_at": "2016-10-21T15:04:00.337Z",
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
    },
    {
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 248,
      "chapter_id": 48,
      "position": 60,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:00.749Z",
      "created_at": "2016-10-21T15:04:00.633Z",
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e69c4f61cfe287df14d8c24398b1e0b9314f9b4340207c199a4cffa4e4be4e98"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer b249a0c7a60213e01e7f3c792bda3d2ff3064d9de00d62465330882ca45352bc
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 264,
      "chapter_id": 53,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:02.283Z",
      "created_at": "2016-10-21T15:04:02.165Z",
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
          "id": 129,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 130,
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
	-H "Authorization: Bearer b249a0c7a60213e01e7f3c792bda3d2ff3064d9de00d62465330882ca45352bc"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/75/republish
Content-Type: application/json
Authorization: Bearer e36b83c21d9437f9fd8583db0e68cef506f8a556680b43e592b7e9f921e5f235
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/75/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e36b83c21d9437f9fd8583db0e68cef506f8a556680b43e592b7e9f921e5f235"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a075d965c3ad7669151a324e0a63ff653db2ed8554287ef95cdf14d5d81cbb13
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}
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
    "creator_id": 113,
    "id": 40,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 40,
    "additional_university_ids": [

    ],
    "topic_id": 40,
    "discipline_id": 40,
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
    "updated_at": "2016-10-21T15:03:49.165Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a075d965c3ad7669151a324e0a63ff653db2ed8554287ef95cdf14d5d81cbb13"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b436e46e4365e04998d624ec136a5f544f89c55c8d51aece13e12b6a36638d42
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
      "creator_id": 145,
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-40",
      "html_url": "https://goskive.com/course/fu-course-40",
      "slug": "fu-course-40",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "topic_id": 69,
      "discipline_id": 69,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 40",
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
      "updated_at": "2016-10-21T15:03:52.096Z",
      "shortname": "fu-course-40"
    },
    {
      "creator_id": 145,
      "id": 70,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "topic_id": 70,
      "discipline_id": 70,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
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
      "updated_at": "2016-10-21T15:03:52.137Z",
      "shortname": "fu-course-41"
    },
    {
      "creator_id": 146,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "topic_id": 71,
      "discipline_id": 71,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
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
      "updated_at": "2016-10-21T15:03:52.186Z",
      "shortname": "fu-course-42"
    },
    {
      "creator_id": 146,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-43",
      "html_url": "https://goskive.com/course/fu-course-43",
      "slug": "fu-course-43",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "topic_id": 72,
      "discipline_id": 72,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 43",
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
      "chapters_updated_at": "2016-10-21T15:03:52.482Z",
      "updated_at": "2016-10-21T15:03:52.489Z",
      "shortname": "fu-course-43"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b436e46e4365e04998d624ec136a5f544f89c55c8d51aece13e12b6a36638d42"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d1fe3b6ea996403f55bf32fd92f5ceb208cad5942581ca7962e3fd2193d7fe9b
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
      "creator_id": 152,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 73,
      "discipline_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 44",
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
      "updated_at": "2016-10-21T15:03:52.696Z",
      "shortname": "fu-course-44"
    },
    {
      "creator_id": 152,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 45",
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
      "updated_at": "2016-10-21T15:03:52.737Z",
      "shortname": "fu-course-45"
    },
    {
      "creator_id": 153,
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 46",
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
      "updated_at": "2016-10-21T15:03:52.786Z",
      "shortname": "fu-course-46"
    },
    {
      "creator_id": 153,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 76,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
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
      "updated_at": "2016-10-21T15:03:52.828Z",
      "shortname": "fu-course-47"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1fe3b6ea996403f55bf32fd92f5ceb208cad5942581ca7962e3fd2193d7fe9b"
```
