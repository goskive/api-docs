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
DELETE /v2/chapters/187
Content-Type: application/json
Authorization: Bearer 8d0876da299d04914a988dad21c48064bd418550aa132a16bfc4ea40707cc6cd
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/187" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d0876da299d04914a988dad21c48064bd418550aa132a16bfc4ea40707cc6cd"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/183
Content-Type: application/json
Authorization: Bearer fcd1a5c17d2e2222a5428b7c86a813c13e225fb44a44c146e3728b0a41b08a45
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
    "id": 183,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T12:29:53.115Z",
    "course_id": 289,
    "author_id": 913,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-26T12:29:52.590Z",
    "questions_updated_at": "2016-10-26T12:29:52.590Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 916,
        "chapter_id": 183,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:53.063Z",
        "created_at": "2016-10-26T12:29:53.063Z",
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
        "author_id": 917,
        "chapter_id": 183,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:53.099Z",
        "created_at": "2016-10-26T12:29:53.099Z",
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
        "id": 127,
        "obfuscated_id": "E3yfRgAzssw",
        "author_id": 914,
        "chapter_id": 183,
        "position": 114,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:52.804Z",
        "created_at": "2016-10-26T12:29:52.696Z",
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
            "id": 257,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 258,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 128,
        "obfuscated_id": "Q4ODZIcqv0E",
        "author_id": 915,
        "chapter_id": 183,
        "position": 115,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:52.994Z",
        "created_at": "2016-10-26T12:29:52.875Z",
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
            "id": 259,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 260,
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
curl "api.goskive.com/v2/chapters/183" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcd1a5c17d2e2222a5428b7c86a813c13e225fb44a44c146e3728b0a41b08a45"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/184
Content-Type: application/json
Authorization: Bearer af72d932033af52b11175b4524f2955f224359cdc5c29bcefaacd5ed0167ca81
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
    "id": 184,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T12:29:53.324Z",
    "course_id": 290,
    "author_id": 920,
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
curl "api.goskive.com/v2/chapters/184" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af72d932033af52b11175b4524f2955f224359cdc5c29bcefaacd5ed0167ca81"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 174da9472c139dbc37d77b0762c121543fc5b4eddde79e95ae42ab0ea51f1d39
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 174da9472c139dbc37d77b0762c121543fc5b4eddde79e95ae42ab0ea51f1d39"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 406015e24b75e6512be22e99fdeabc0cf5ac619b667f8c0d29038442c7872768
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
      "id": 5,
      "author_id": 640,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:35.052Z",
      "status": "published",
      "subject_id": 205,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 642,
      "reply_to_id": 5,
      "created_at": "2016-10-26T12:29:35.137Z",
      "status": "published",
      "subject_id": 206,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 644,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:35.221Z",
      "status": "published",
      "subject_id": 207,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 8,
      "author_id": 646,
      "reply_to_id": 7,
      "created_at": "2016-10-26T12:29:35.304Z",
      "status": "published",
      "subject_id": 208,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 648,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:35.387Z",
      "status": "reported",
      "subject_id": 209,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 650,
      "reply_to_id": 9,
      "created_at": "2016-10-26T12:29:35.471Z",
      "status": "published",
      "subject_id": 210,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 652,
      "reply_to_id": 9,
      "created_at": "2016-10-26T12:29:35.555Z",
      "status": "published",
      "subject_id": 211,
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
	-H "Authorization: Bearer 406015e24b75e6512be22e99fdeabc0cf5ac619b667f8c0d29038442c7872768"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 9cff7eaafe8fe0568893e5383476b25f9034dcd035d4ced90e677bdc69c07318
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
      "id": 19,
      "author_id": 670,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:36.301Z",
      "status": "published",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 672,
      "reply_to_id": 19,
      "created_at": "2016-10-26T12:29:36.380Z",
      "status": "published",
      "subject_id": 220,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 674,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:36.461Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 676,
      "reply_to_id": 21,
      "created_at": "2016-10-26T12:29:36.540Z",
      "status": "published",
      "subject_id": 222,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 678,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:36.621Z",
      "status": "reported",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 680,
      "reply_to_id": 23,
      "created_at": "2016-10-26T12:29:36.702Z",
      "status": "published",
      "subject_id": 224,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 682,
      "reply_to_id": 23,
      "created_at": "2016-10-26T12:29:36.783Z",
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
	-H "Authorization: Bearer 9cff7eaafe8fe0568893e5383476b25f9034dcd035d4ced90e677bdc69c07318"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer cae05a6fd44cb7f8cc66de2a5227db328fc0a154d10a28fe3c3ab81ac4208867
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
      "id": 34,
      "author_id": 702,
      "reply_to_id": 33,
      "created_at": "2016-10-26T12:29:37.640Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 706,
      "reply_to_id": 35,
      "created_at": "2016-10-26T12:29:37.801Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 710,
      "reply_to_id": 37,
      "created_at": "2016-10-26T12:29:37.961Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 712,
      "reply_to_id": 37,
      "created_at": "2016-10-26T12:29:38.042Z",
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
	-H "Authorization: Bearer cae05a6fd44cb7f8cc66de2a5227db328fc0a154d10a28fe3c3ab81ac4208867"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 4dfa35b63b08fbd4104dffd2a1cb3123b2ed15239a67a17b44d7e07ce659cb5b
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
      "id": 16,
      "author_id": 663,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:36.023Z",
      "status": "reported",
      "subject_id": 216,
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
	-H "Authorization: Bearer 4dfa35b63b08fbd4104dffd2a1cb3123b2ed15239a67a17b44d7e07ce659cb5b"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/41/republish
Content-Type: application/json
Authorization: Bearer 34f5a70c8f5050a6cfd5e1d7355099497c1fe1423b106ae77f5e044ba3ef28b4
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
	-H "Authorization: Bearer 34f5a70c8f5050a6cfd5e1d7355099497c1fe1423b106ae77f5e044ba3ef28b4"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 77c8f8d2a15a4f8861b64c20699ff6ae96c653c779cb37d55f66f06bb1222dae
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
    "id": 119,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T12:29:30.418Z",
    "course_id": 186,
    "author_id": 562,
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
	-H "Authorization: Bearer 77c8f8d2a15a4f8861b64c20699ff6ae96c653c779cb37d55f66f06bb1222dae"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/187/chapters
Content-Type: application/json
Authorization: Bearer 98c542df232dadf2596701ee9ae00652c7fc38b23555bfadbb16b76461387a56
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
    "id": 120,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T12:29:30.545Z",
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
curl "api.goskive.com/v2/courses/187/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98c542df232dadf2596701ee9ae00652c7fc38b23555bfadbb16b76461387a56"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7f2f1f25e88917e88fea751951b517bdba7487fadf31c7331a16efe8c23baf37
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
      "title": "Clever Chapter Title 124",
      "position": 1,
      "updated_at": "2016-10-26T12:29:32.329Z",
      "course_id": 196,
      "author_id": 598,
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
      "title": "Clever Chapter Title 125",
      "position": 2,
      "updated_at": "2016-10-26T12:29:32.353Z",
      "course_id": 196,
      "author_id": 599,
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
      "title": "Clever Chapter Title 126",
      "position": 3,
      "updated_at": "2016-10-26T12:29:32.604Z",
      "course_id": 196,
      "author_id": 600,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-26T12:29:32.254Z",
      "questions_updated_at": "2016-10-26T12:29:32.254Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f2f1f25e88917e88fea751951b517bdba7487fadf31c7331a16efe8c23baf37"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer dd89487e9c6d59d7b1d5dc5c61085e9652d0e2d3f8e7d22a6951ee801ed0aab0
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
      "id": 139,
      "title": "Clever Chapter Title 127",
      "position": 1,
      "updated_at": "2016-10-26T12:29:32.768Z",
      "course_id": 197,
      "author_id": 605,
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
      "id": 140,
      "title": "Clever Chapter Title 128",
      "position": 2,
      "updated_at": "2016-10-26T12:29:32.791Z",
      "course_id": 197,
      "author_id": 606,
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
      "id": 141,
      "title": "Clever Chapter Title 129",
      "position": 3,
      "updated_at": "2016-10-26T12:29:32.815Z",
      "course_id": 197,
      "author_id": 607,
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
	-H "Authorization: Bearer dd89487e9c6d59d7b1d5dc5c61085e9652d0e2d3f8e7d22a6951ee801ed0aab0"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/131
Content-Type: application/json
Authorization: Bearer a644f4b76cabc1d9971b0e6faa886bff1df3527c5a593fa828a69b0f02954bcd
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/131" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a644f4b76cabc1d9971b0e6faa886bff1df3527c5a593fa828a69b0f02954bcd"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 96ef668fbbfd1b20ea9e9a84bd8d8277048ff174dd2a49b45398832e1f33734d
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
	-H "Authorization: Bearer 96ef668fbbfd1b20ea9e9a84bd8d8277048ff174dd2a49b45398832e1f33734d"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer b78c395487449346b126233b2e23707140a65f397cceffc8733010a5c4f06293
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
    "creator_id": 357,
    "id": 129,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 113,
    "additional_university_ids": [

    ],
    "topic_id": 136,
    "discipline_id": 137,
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
    "chapters_updated_at": "2016-10-26T12:29:13.890Z",
    "updated_at": "2016-10-26T12:29:15.298Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 78,
        "title": "Clever Chapter Title 69",
        "position": 1,
        "updated_at": "2016-10-26T12:29:15.253Z",
        "course_id": 129,
        "author_id": 357,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T12:29:13.890Z",
        "questions_updated_at": "2016-10-26T12:29:13.890Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 79,
        "title": "Clever Chapter Title 70",
        "position": 2,
        "updated_at": "2016-10-26T12:29:15.291Z",
        "course_id": 129,
        "author_id": 357,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T12:29:13.890Z",
        "questions_updated_at": "2016-10-26T12:29:13.890Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 357,
        "chapter_id": 78,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.098Z",
        "created_at": "2016-10-26T12:29:15.098Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 357,
        "chapter_id": 79,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.167Z",
        "created_at": "2016-10-26T12:29:15.167Z",
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
        "author_id": 357,
        "chapter_id": 78,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.137Z",
        "created_at": "2016-10-26T12:29:15.137Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 357,
        "chapter_id": 79,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.206Z",
        "created_at": "2016-10-26T12:29:15.206Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 360,
        "chapter_id": 78,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.244Z",
        "created_at": "2016-10-26T12:29:15.244Z",
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
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 361,
        "chapter_id": 79,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.281Z",
        "created_at": "2016-10-26T12:29:15.281Z",
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
	-H "Authorization: Bearer b78c395487449346b126233b2e23707140a65f397cceffc8733010a5c4f06293"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/143
Content-Type: application/json
Authorization: Bearer 7ef9666d32e89ef7c1e08d8472beb79e2a40e70ebeb1aeb66143e3ba83d39f76
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
    "creator_id": 394,
    "id": 143,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 127,
    "additional_university_ids": [

    ],
    "topic_id": 150,
    "discipline_id": 151,
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
    "updated_at": "2016-10-26T12:29:18.929Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/143" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ef9666d32e89ef7c1e08d8472beb79e2a40e70ebeb1aeb66143e3ba83d39f76"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 80321dc8d72713f433bfba1e1b3ea4047fd5184c78a66b6e0e9d94c51e768cc9
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
    "creator_id": 389,
    "id": 140,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 124,
    "additional_university_ids": [

    ],
    "topic_id": 147,
    "discipline_id": 148,
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
    "updated_at": "2016-10-26T12:29:18.569Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80321dc8d72713f433bfba1e1b3ea4047fd5184c78a66b6e0e9d94c51e768cc9"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 66d3e0d499cf9f5559e86e1a28ea9c9a758722a31f035e7bafa7dffb6a266de5
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
      "id": 7,
      "user_id": 462,
      "feedbackable_id": 78,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:23.548Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 466,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:23.831Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 470,
      "feedbackable_id": 80,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:24.119Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 474,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:24.411Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 478,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T12:29:24.703Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66d3e0d499cf9f5559e86e1a28ea9c9a758722a31f035e7bafa7dffb6a266de5"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 72e9074a53bb06b97846a9514125d592b6f8b2996a8ca5bec24518bdf7bc21ab
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
      "id": 16,
      "user_id": 499,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T12:29:26.181Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72e9074a53bb06b97846a9514125d592b6f8b2996a8ca5bec24518bdf7bc21ab"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer de703aa4f5da59b0c44ab95dab10009cfb8981f5c8c4d8c708adcef1e0f876eb
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de703aa4f5da59b0c44ab95dab10009cfb8981f5c8c4d8c708adcef1e0f876eb"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/4/metadata
Content-Type: application/json
Authorization: Bearer 4c346dcf25d39e7584f5a0a7fd92a9934b3174ace3e4e4b790b229d70fe6e195
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
      "id": 316,
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
      "created_at": "2016-10-26T12:29:09.342Z",
      "updated_at": "2016-10-26T12:29:09.342Z"
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
    "created_at": "2016-10-26T12:29:09.414Z",
    "updated_at": "2016-10-26T12:29:09.414Z",
    "course_id": 116,
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
	-H "Authorization: Bearer 4c346dcf25d39e7584f5a0a7fd92a9934b3174ace3e4e4b790b229d70fe6e195"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/83/feedbacks
Content-Type: application/json
Authorization: Bearer a7ee1b4cbc32a32ae4f1c71d2da2639ab9279692696867f054687feead7fadbb
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
      "id": 40,
      "user_id": 863,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:49.561Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 862,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:49.551Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7ee1b4cbc32a32ae4f1c71d2da2639ab9279692696867f054687feead7fadbb"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer bde576b1a8efaf8ec12c9ca43f2b49933ca8d1085bae1171c13eac4a58b8437a
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
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 21,
      "chapter_id": 7,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:41.752Z",
      "created_at": "2016-10-26T12:28:41.752Z",
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
      "id": 8,
      "obfuscated_id": "X2B_8FVuFe8",
      "author_id": 24,
      "chapter_id": 8,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:41.876Z",
      "created_at": "2016-10-26T12:28:41.876Z",
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
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 27,
      "chapter_id": 9,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:41.999Z",
      "created_at": "2016-10-26T12:28:41.999Z",
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
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 30,
      "chapter_id": 10,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:42.124Z",
      "created_at": "2016-10-26T12:28:42.124Z",
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 33,
      "chapter_id": 11,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:42.248Z",
      "created_at": "2016-10-26T12:28:42.248Z",
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
	-H "Authorization: Bearer bde576b1a8efaf8ec12c9ca43f2b49933ca8d1085bae1171c13eac4a58b8437a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 3fa34734cecf8a6e561d32877bfd4801e5b5ab4b85b38298e05115f8fa176425
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 49,
      "chapter_id": 16,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:42.922Z",
      "created_at": "2016-10-26T12:28:42.922Z",
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
	-H "Authorization: Bearer 3fa34734cecf8a6e561d32877bfd4801e5b5ab4b85b38298e05115f8fa176425"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/3/republish
Content-Type: application/json
Authorization: Bearer 0e41bc6433642519de9a833401b90bdf3527ca2266cf384c8b2323844d079c96
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/3/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e41bc6433642519de9a833401b90bdf3527ca2266cf384c8b2323844d079c96"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/114/feedbacks
Content-Type: application/json
Authorization: Bearer cd1522cbdf0ff1c71dad962c9302882cdd47e1cf15ece1059dcbbe20c131e354
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
      "user_id": 797,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:44.442Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 796,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:44.429Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/114/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd1522cbdf0ff1c71dad962c9302882cdd47e1cf15ece1059dcbbe20c131e354"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer f16891a384efe7fdb198ef62e7c93c2b4e0b09984f86ad4cb677f663be203275
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 248,
      "chapter_id": 55,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:01.928Z",
      "created_at": "2016-10-26T12:29:01.798Z",
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
          "id": 69,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 70,
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
      "author_id": 239,
      "chapter_id": 52,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:00.997Z",
      "created_at": "2016-10-26T12:29:00.860Z",
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
          "id": 63,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 64,
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
      "author_id": 236,
      "chapter_id": 51,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:00.688Z",
      "created_at": "2016-10-26T12:29:00.552Z",
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
          "id": 61,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 62,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 242,
      "chapter_id": 53,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:01.309Z",
      "created_at": "2016-10-26T12:29:01.168Z",
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
          "id": 65,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 66,
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
      "author_id": 245,
      "chapter_id": 54,
      "position": 26,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:01.624Z",
      "created_at": "2016-10-26T12:29:01.482Z",
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
          "id": 67,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 68,
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
	-H "Authorization: Bearer f16891a384efe7fdb198ef62e7c93c2b4e0b09984f86ad4cb677f663be203275"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 861660bf522f881b1d359c51f7cf2d844ce50234a4f99cce527ee06f1b7e5415
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
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 280,
      "chapter_id": 65,
      "position": 37,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:05.213Z",
      "created_at": "2016-10-26T12:29:05.074Z",
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
          "id": 89,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 90,
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
	-H "Authorization: Bearer 861660bf522f881b1d359c51f7cf2d844ce50234a4f99cce527ee06f1b7e5415"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/47/republish
Content-Type: application/json
Authorization: Bearer 41ca093496da872271a5cf4fab74ad65cc78148dff6b39d6ab56671c7a0e9125
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
	-H "Authorization: Bearer 41ca093496da872271a5cf4fab74ad65cc78148dff6b39d6ab56671c7a0e9125"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d0780edfc967c5a0e0bd92f91807c39a060b6d6bc86cb8173081c9bd36239c24
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":57,"published":false}}
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
    "creator_id": 172,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 51,
    "additional_university_ids": [

    ],
    "topic_id": 57,
    "discipline_id": 58,
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
    "updated_at": "2016-10-26T12:28:53.810Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":57,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0780edfc967c5a0e0bd92f91807c39a060b6d6bc86cb8173081c9bd36239c24"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e4a9b9418de52047b99c85f7fd0594c3cafe32c6f29c6b4a97ad2d2dbbf3460b
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
      "creator_id": 186,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-40",
      "html_url": "https://goskive.com/course/fu-course-40",
      "slug": "fu-course-40",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 69,
      "discipline_id": 70,
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
      "updated_at": "2016-10-26T12:28:55.188Z",
      "shortname": "fu-course-40"
    },
    {
      "creator_id": 186,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 70,
      "discipline_id": 71,
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
      "updated_at": "2016-10-26T12:28:55.225Z",
      "shortname": "fu-course-41"
    },
    {
      "creator_id": 187,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 71,
      "discipline_id": 72,
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
      "updated_at": "2016-10-26T12:28:55.269Z",
      "shortname": "fu-course-42"
    },
    {
      "creator_id": 187,
      "id": 65,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-43",
      "html_url": "https://goskive.com/course/fu-course-43",
      "slug": "fu-course-43",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 72,
      "discipline_id": 73,
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
      "chapters_updated_at": "2016-10-26T12:28:55.568Z",
      "updated_at": "2016-10-26T12:28:55.575Z",
      "shortname": "fu-course-43"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4a9b9418de52047b99c85f7fd0594c3cafe32c6f29c6b4a97ad2d2dbbf3460b"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5d57feeebb709b8f9684461b688b7d423d33b57fcdc602a3e9fee30e0333a399
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
      "creator_id": 193,
      "id": 66,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 73,
      "discipline_id": 74,
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
      "updated_at": "2016-10-26T12:28:55.768Z",
      "shortname": "fu-course-44"
    },
    {
      "creator_id": 193,
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 75,
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
      "updated_at": "2016-10-26T12:28:55.804Z",
      "shortname": "fu-course-45"
    },
    {
      "creator_id": 194,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 76,
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
      "updated_at": "2016-10-26T12:28:55.848Z",
      "shortname": "fu-course-46"
    },
    {
      "creator_id": 194,
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 77,
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
      "updated_at": "2016-10-26T12:28:55.885Z",
      "shortname": "fu-course-47"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d57feeebb709b8f9684461b688b7d423d33b57fcdc602a3e9fee30e0333a399"
```
