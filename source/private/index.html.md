---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Chapters

## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/34
Content-Type: application/json
Authorization: Bearer 37f279f8728980de6793d3ccfe73fea095f2a95aad7ea749f391e849dd781a3d
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/34" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37f279f8728980de6793d3ccfe73fea095f2a95aad7ea749f391e849dd781a3d"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/29
Content-Type: application/json
Authorization: Bearer a1ac19565c33112e92a911e6d888b64a7559706dfcd5451bf5ae9c8e7fa885d0
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
    "id": 29,
    "updated_at": "2016-12-15T17:19:36.866Z",
    "course_id": 31,
    "author_id": 99,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-15T17:19:36.351Z",
    "questions_updated_at": "2016-12-15T17:19:36.351Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 102,
        "chapter_id": 29,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:36.807Z",
        "created_at": "2016-12-15T17:19:36.807Z",
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
        "author_id": 103,
        "chapter_id": 29,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:36.847Z",
        "created_at": "2016-12-15T17:19:36.847Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 100,
        "chapter_id": 29,
        "position": 5,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:36.583Z",
        "created_at": "2016-12-15T17:19:36.503Z",
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
            "id": 9,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 10,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 101,
        "chapter_id": 29,
        "position": 6,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:36.741Z",
        "created_at": "2016-12-15T17:19:36.650Z",
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
            "id": 11,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 12,
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
curl "api.goskive.com/v2/chapters/29" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1ac19565c33112e92a911e6d888b64a7559706dfcd5451bf5ae9c8e7fa885d0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/31
Content-Type: application/json
Authorization: Bearer 194c304d762f867be2568e40b65b6262ec896dd7360fad13b8881ec4c5d3af46
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
    "id": 31,
    "updated_at": "2016-12-15T17:19:37.789Z",
    "course_id": 33,
    "author_id": 113,
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
curl "api.goskive.com/v2/chapters/31" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 194c304d762f867be2568e40b65b6262ec896dd7360fad13b8881ec4c5d3af46"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/57
Content-Type: application/json
Authorization: Bearer 45e8ba540af028f0749d978583a6701e1bc31aac15e041414fa25d7e4a48ef76
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45e8ba540af028f0749d978583a6701e1bc31aac15e041414fa25d7e4a48ef76"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2054a0f1e212944a3723b68be957e91689342ee07e389aac4206261f90446a8b
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
      "id": 20,
      "author_id": 871,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:51.931Z",
      "status": "published",
      "subject_id": 268,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 873,
      "reply_to_id": 20,
      "created_at": "2016-12-15T17:20:52.063Z",
      "status": "published",
      "subject_id": 269,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 875,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:52.198Z",
      "status": "published",
      "subject_id": 270,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 877,
      "reply_to_id": 22,
      "created_at": "2016-12-15T17:20:52.327Z",
      "status": "published",
      "subject_id": 271,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 879,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:52.459Z",
      "status": "reported",
      "subject_id": 272,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 881,
      "reply_to_id": 24,
      "created_at": "2016-12-15T17:20:52.593Z",
      "status": "published",
      "subject_id": 273,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 883,
      "reply_to_id": 24,
      "created_at": "2016-12-15T17:20:52.722Z",
      "status": "published",
      "subject_id": 274,
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
	-H "Authorization: Bearer 2054a0f1e212944a3723b68be957e91689342ee07e389aac4206261f90446a8b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer fc979a748cd9f1c81e20f7fefe9c59cf49b31735cf42bdea8aecd36d5ab02a6f
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
      "author_id": 886,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:52.921Z",
      "status": "published",
      "subject_id": 275,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 888,
      "reply_to_id": 27,
      "created_at": "2016-12-15T17:20:53.057Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 890,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:53.188Z",
      "status": "published",
      "subject_id": 277,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 892,
      "reply_to_id": 29,
      "created_at": "2016-12-15T17:20:53.317Z",
      "status": "published",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 894,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:53.455Z",
      "status": "reported",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 896,
      "reply_to_id": 31,
      "created_at": "2016-12-15T17:20:53.586Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 898,
      "reply_to_id": 31,
      "created_at": "2016-12-15T17:20:53.717Z",
      "status": "published",
      "subject_id": 281,
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
	-H "Authorization: Bearer fc979a748cd9f1c81e20f7fefe9c59cf49b31735cf42bdea8aecd36d5ab02a6f"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 367fcdc8529036d36d831f25ddcfe44f905cb199c113f7fe19bbf4564a269501
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
      "id": 35,
      "author_id": 903,
      "reply_to_id": 34,
      "created_at": "2016-12-15T17:20:54.080Z",
      "status": "published",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 907,
      "reply_to_id": 36,
      "created_at": "2016-12-15T17:20:54.344Z",
      "status": "published",
      "subject_id": 285,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 911,
      "reply_to_id": 38,
      "created_at": "2016-12-15T17:20:54.613Z",
      "status": "published",
      "subject_id": 287,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 913,
      "reply_to_id": 38,
      "created_at": "2016-12-15T17:20:54.744Z",
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
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 367fcdc8529036d36d831f25ddcfe44f905cb199c113f7fe19bbf4564a269501"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 83ec381ee352b97b28510fa4094b4aff80235a53cfbf4a7c673906e4f5104d4a
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
      "id": 45,
      "author_id": 924,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:55.459Z",
      "status": "reported",
      "subject_id": 293,
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
	-H "Authorization: Bearer 83ec381ee352b97b28510fa4094b4aff80235a53cfbf4a7c673906e4f5104d4a"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/59/republish
Content-Type: application/json
Authorization: Bearer 8ba9c70bfb9dee82e3b93b0ce1ac75ba836baa18eeb3bc15dd9b82af2609e9dd
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/59/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ba9c70bfb9dee82e3b93b0ce1ac75ba836baa18eeb3bc15dd9b82af2609e9dd"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 831454f35438729c9532d46fa91aeed0d37c7507c5ec7d3607e812a634ab0410
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
    "id": 91,
    "updated_at": "2016-12-15T17:20:01.681Z",
    "course_id": 97,
    "author_id": 374,
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
	-H "Authorization: Bearer 831454f35438729c9532d46fa91aeed0d37c7507c5ec7d3607e812a634ab0410"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/100/chapters
Content-Type: application/json
Authorization: Bearer 42d0e0569d73e0003f102252c35b558c0e006a660c568a084dc29a8ce5d70b00
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
    "id": 93,
    "updated_at": "2016-12-15T17:20:02.232Z",
    "course_id": 100,
    "author_id": 380,
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
curl "api.goskive.com/v2/courses/100/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42d0e0569d73e0003f102252c35b558c0e006a660c568a084dc29a8ce5d70b00"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer df3f892c67adb4fb64f55e2ce0282b1aa4b4f9815bbdc477db39b55ee14746c5
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
      "id": 73,
      "updated_at": "2016-12-15T17:19:58.758Z",
      "course_id": 88,
      "author_id": 335,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 64",
      "position": 1
    },
    {
      "id": 74,
      "updated_at": "2016-12-15T17:19:58.788Z",
      "course_id": 88,
      "author_id": 336,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 65",
      "position": 2
    },
    {
      "id": 75,
      "updated_at": "2016-12-15T17:19:59.049Z",
      "course_id": 88,
      "author_id": 337,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-15T17:19:58.629Z",
      "questions_updated_at": "2016-12-15T17:19:58.629Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 66",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df3f892c67adb4fb64f55e2ce0282b1aa4b4f9815bbdc477db39b55ee14746c5"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 85af2148ff1f6b9c1c3600ceda54e2beb1240c64026fee27a60ffa347913d778
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
      "id": 76,
      "updated_at": "2016-12-15T17:19:59.282Z",
      "course_id": 89,
      "author_id": 342,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 67",
      "position": 1
    },
    {
      "id": 77,
      "updated_at": "2016-12-15T17:19:59.310Z",
      "course_id": 89,
      "author_id": 343,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 68",
      "position": 2
    },
    {
      "id": 78,
      "updated_at": "2016-12-15T17:19:59.339Z",
      "course_id": 89,
      "author_id": 344,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 69",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85af2148ff1f6b9c1c3600ceda54e2beb1240c64026fee27a60ffa347913d778"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b821658c7eaec58bea24d3ae1cc20d663f6fc7a4c35fab6c54751f7016137db1
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
	-H "Authorization: Bearer b821658c7eaec58bea24d3ae1cc20d663f6fc7a4c35fab6c54751f7016137db1"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/254
Content-Type: application/json
Authorization: Bearer 22a3699fceadc0f05e7e7f3ae8e65cf2c1df1cefaba4ebb3e8c40d705c90de6f
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/254" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22a3699fceadc0f05e7e7f3ae8e65cf2c1df1cefaba4ebb3e8c40d705c90de6f"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4835c028b1229c900efa4150c839e44da786b1107643fe02c10ab7424f627e9f
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
    "creator_id": 785,
    "id": 242,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 226,
    "additional_university_ids": [

    ],
    "discipline_id": 244,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 6,
    "questions_count": 6,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-15T17:20:40.916Z",
    "updated_at": "2016-12-15T17:20:42.189Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 785,
        "chapter_id": 175,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:41.961Z",
        "created_at": "2016-12-15T17:20:41.961Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 785,
        "chapter_id": 176,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:42.037Z",
        "created_at": "2016-12-15T17:20:42.037Z",
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
        "author_id": 785,
        "chapter_id": 175,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:42.004Z",
        "created_at": "2016-12-15T17:20:42.004Z",
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
        "author_id": 785,
        "chapter_id": 176,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:42.082Z",
        "created_at": "2016-12-15T17:20:42.082Z",
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
        "author_id": 788,
        "chapter_id": 175,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:42.127Z",
        "created_at": "2016-12-15T17:20:42.127Z",
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
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 789,
        "chapter_id": 176,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:42.168Z",
        "created_at": "2016-12-15T17:20:42.168Z",
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
        "id": 175,
        "updated_at": "2016-12-15T17:20:42.137Z",
        "course_id": 242,
        "author_id": 785,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T17:20:40.916Z",
        "questions_updated_at": "2016-12-15T17:20:40.916Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 157",
        "position": 1
      },
      {
        "id": 176,
        "updated_at": "2016-12-15T17:20:42.179Z",
        "course_id": 242,
        "author_id": 785,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T17:20:40.916Z",
        "questions_updated_at": "2016-12-15T17:20:40.916Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 158",
        "position": 2
      }
    ],
    "topic_id": 244,
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
	-H "Authorization: Bearer 4835c028b1229c900efa4150c839e44da786b1107643fe02c10ab7424f627e9f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/236
Content-Type: application/json
Authorization: Bearer 154a67dd2b35094a2c7df47ee62495073edd2135e130c99f7e0c7a0ea1e1997c
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
    "creator_id": 767,
    "id": 236,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 220,
    "additional_university_ids": [

    ],
    "discipline_id": 238,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-15T17:20:37.509Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 238,
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
curl "api.goskive.com/v2/courses/236" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 154a67dd2b35094a2c7df47ee62495073edd2135e130c99f7e0c7a0ea1e1997c"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b9ef87833647d1e68f922de05b29594eb9e85cfb92ec2128806c97690a319111
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
    "creator_id": 770,
    "id": 238,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 222,
    "additional_university_ids": [

    ],
    "discipline_id": 240,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-15T17:20:37.939Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 240,
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
	-H "Authorization: Bearer b9ef87833647d1e68f922de05b29594eb9e85cfb92ec2128806c97690a319111"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 61a4b62468acb0b9014584cf01da24bdbe2c5352d0450c10c9e3323b292e8f65
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
      "id": 14,
      "user_id": 610,
      "feedbackable_id": 72,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:25.614Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 614,
      "feedbackable_id": 73,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:25.927Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 618,
      "feedbackable_id": 74,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:26.235Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 622,
      "feedbackable_id": 75,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:26.540Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 626,
      "feedbackable_id": 76,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T17:20:26.849Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61a4b62468acb0b9014584cf01da24bdbe2c5352d0450c10c9e3323b292e8f65"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer bc2d245972fa45f5f9d73c3eff125e3e0a60e41e2a31793b5d63449f503856a6
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
      "user_id": 684,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T17:20:31.366Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc2d245972fa45f5f9d73c3eff125e3e0a60e41e2a31793b5d63449f503856a6"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer 2153c4000679dfb153203143efd3eab003fc5f6a55528797db4f6e2b723a1a7a
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
	-H "Authorization: Bearer 2153c4000679dfb153203143efd3eab003fc5f6a55528797db4f6e2b723a1a7a"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/15/metadata
Content-Type: application/json
Authorization: Bearer 0ad6ab776ee00ed3ad66b5faf48c00555af12d91e6160aa59251dd50dc246816
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
    "id": 15,
    "uploader": {
      "id": 485,
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
      "created_at": "2016-12-15T17:20:12.298Z",
      "updated_at": "2016-12-15T17:20:12.298Z"
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
    "created_at": "2016-12-15T17:20:12.422Z",
    "updated_at": "2016-12-15T17:20:12.422Z",
    "course_id": 161,
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
curl "api.goskive.com/v2/files/15/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ad6ab776ee00ed3ad66b5faf48c00555af12d91e6160aa59251dd50dc246816"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/69/feedbacks
Content-Type: application/json
Authorization: Bearer 0faea2eb5fa04e28db133134b8ab6cd2bd7a4e09522609f8f6dd31a9aa633605
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
      "user_id": 732,
      "feedbackable_id": 69,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:34.748Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 731,
      "feedbackable_id": 69,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:34.737Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/69/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0faea2eb5fa04e28db133134b8ab6cd2bd7a4e09522609f8f6dd31a9aa633605"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer b9168d8f8d26e87a34ab408e06c8053a63301c33f59528f2e60de7b45ed9a508
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 65,
      "chapter_id": 18,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:34.294Z",
      "created_at": "2016-12-15T17:19:34.294Z",
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 68,
      "chapter_id": 19,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:34.486Z",
      "created_at": "2016-12-15T17:19:34.486Z",
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 71,
      "chapter_id": 20,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:34.673Z",
      "created_at": "2016-12-15T17:19:34.673Z",
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 74,
      "chapter_id": 21,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:34.883Z",
      "created_at": "2016-12-15T17:19:34.883Z",
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
      "author_id": 77,
      "chapter_id": 22,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:35.067Z",
      "created_at": "2016-12-15T17:19:35.067Z",
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
	-H "Authorization: Bearer b9168d8f8d26e87a34ab408e06c8053a63301c33f59528f2e60de7b45ed9a508"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 6cabb7fd1a64b35d045b7f3ae5234e86f04188ab6bd515b8553a9b974860564b
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 61,
      "chapter_id": 17,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:19:34.069Z",
      "created_at": "2016-12-15T17:19:34.069Z",
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
	-H "Authorization: Bearer 6cabb7fd1a64b35d045b7f3ae5234e86f04188ab6bd515b8553a9b974860564b"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/7/republish
Content-Type: application/json
Authorization: Bearer a59293e1b62f1e9612868cb458f5f8bdf60b790347d8d9940b93a333f5a7e6dd
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/7/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a59293e1b62f1e9612868cb458f5f8bdf60b790347d8d9940b93a333f5a7e6dd"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/13/feedbacks
Content-Type: application/json
Authorization: Bearer a1a54319c603c11275864693654a76bab08ebb498201626d3fb7f9d8e489bd8d
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
      "user_id": 149,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:19:41.736Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 148,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:19:41.726Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/13/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1a54319c603c11275864693654a76bab08ebb498201626d3fb7f9d8e489bd8d"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer ce6ebaa1100faf367245359b2ac7fd01261a9cdf0482bc1a3fa58085beeea493
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 527,
      "chapter_id": 114,
      "position": 51,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:16.346Z",
      "created_at": "2016-12-15T17:20:16.250Z",
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
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 515,
      "chapter_id": 110,
      "position": 47,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:15.026Z",
      "created_at": "2016-12-15T17:20:14.920Z",
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
      "author_id": 518,
      "chapter_id": 111,
      "position": 48,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:15.350Z",
      "created_at": "2016-12-15T17:20:15.244Z",
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 521,
      "chapter_id": 112,
      "position": 49,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:15.676Z",
      "created_at": "2016-12-15T17:20:15.569Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 524,
      "chapter_id": 113,
      "position": 50,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:16.029Z",
      "created_at": "2016-12-15T17:20:15.922Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce6ebaa1100faf367245359b2ac7fd01261a9cdf0482bc1a3fa58085beeea493"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 575e40029a923a80dec0fd94e9f5b39595881098fe618cc6de4e0010a2625b20
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 559,
      "chapter_id": 124,
      "position": 61,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:19.761Z",
      "created_at": "2016-12-15T17:20:19.662Z",
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
          "id": 121,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 122,
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
	-H "Authorization: Bearer 575e40029a923a80dec0fd94e9f5b39595881098fe618cc6de4e0010a2625b20"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/65/republish
Content-Type: application/json
Authorization: Bearer aff2e5f0c031b7328234f4587f82653816b9b3f230ba268791ba392cd9530276
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aff2e5f0c031b7328234f4587f82653816b9b3f230ba268791ba392cd9530276"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9b5348e50738286a38064084cb6402dabc7cf2864108c3b26508e89fd16103a6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":139,"published":false}}
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
    "creator_id": 424,
    "id": 139,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 117,
    "additional_university_ids": [

    ],
    "discipline_id": 139,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-15T17:20:07.226Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 139,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":139,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b5348e50738286a38064084cb6402dabc7cf2864108c3b26508e89fd16103a6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3adf2f24db9d3195bc21c393767d837e2a17a685f78d0ba664d7ce389ceec2fd
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
      "creator_id": 385,
      "id": 105,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-69",
      "html_url": "https://goskive.com/course/fu-course-69",
      "slug": "fu-course-69",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "discipline_id": 105,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:02.823Z",
      "shortname": "fu-course-69",
      "topic_id": 105,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 69",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 385,
      "id": 106,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-70",
      "html_url": "https://goskive.com/course/fu-course-70",
      "slug": "fu-course-70",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "discipline_id": 106,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:02.858Z",
      "shortname": "fu-course-70",
      "topic_id": 106,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 70",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 386,
      "id": 107,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-71",
      "html_url": "https://goskive.com/course/fu-course-71",
      "slug": "fu-course-71",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "discipline_id": 107,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:02.899Z",
      "shortname": "fu-course-71",
      "topic_id": 107,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 71",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 386,
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-72",
      "html_url": "https://goskive.com/course/fu-course-72",
      "slug": "fu-course-72",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "discipline_id": 108,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-15T17:20:02.721Z",
      "updated_at": "2016-12-15T17:20:03.184Z",
      "shortname": "fu-course-72",
      "topic_id": 108,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 72",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3adf2f24db9d3195bc21c393767d837e2a17a685f78d0ba664d7ce389ceec2fd"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 98d351239716c44a5d28cbeb58715a298a3042c919e852787613bf23a23d78fa
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
      "creator_id": 392,
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-73",
      "html_url": "https://goskive.com/course/fu-course-73",
      "slug": "fu-course-73",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 109,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:03.506Z",
      "shortname": "fu-course-73",
      "topic_id": 109,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 73",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 392,
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-74",
      "html_url": "https://goskive.com/course/fu-course-74",
      "slug": "fu-course-74",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 110,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:03.540Z",
      "shortname": "fu-course-74",
      "topic_id": 110,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 74",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 393,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-75",
      "html_url": "https://goskive.com/course/fu-course-75",
      "slug": "fu-course-75",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 111,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:03.583Z",
      "shortname": "fu-course-75",
      "topic_id": 111,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 75",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 393,
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-76",
      "html_url": "https://goskive.com/course/fu-course-76",
      "slug": "fu-course-76",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 112,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-15T17:20:03.618Z",
      "shortname": "fu-course-76",
      "topic_id": 112,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 76",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98d351239716c44a5d28cbeb58715a298a3042c919e852787613bf23a23d78fa"
```
