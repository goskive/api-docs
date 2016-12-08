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
DELETE /v2/chapters/51
Content-Type: application/json
Authorization: Bearer 7a69f349d5332b943af865104b1b75c4ac4c8648325f106e88d1a7f208f43638
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a69f349d5332b943af865104b1b75c4ac4c8648325f106e88d1a7f208f43638"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/53
Content-Type: application/json
Authorization: Bearer 4fff0e79c7a06146df7e7f8b768f1c41e15fe2b148e6e01a7aa5ced34714019c
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
    "id": 53,
    "updated_at": "2016-12-08T18:27:09.881Z",
    "course_id": 114,
    "author_id": 273,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-08T18:27:09.340Z",
    "questions_updated_at": "2016-12-08T18:27:09.340Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 276,
        "chapter_id": 53,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.817Z",
        "created_at": "2016-12-08T18:27:09.817Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 277,
        "chapter_id": 53,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.860Z",
        "created_at": "2016-12-08T18:27:09.860Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 274,
        "chapter_id": 53,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.568Z",
        "created_at": "2016-12-08T18:27:09.476Z",
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
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 275,
        "chapter_id": 53,
        "position": 57,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.746Z",
        "created_at": "2016-12-08T18:27:09.642Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/53" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fff0e79c7a06146df7e7f8b768f1c41e15fe2b148e6e01a7aa5ced34714019c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/47
Content-Type: application/json
Authorization: Bearer c08b6a9aa97a356e921d870de7975e61f8dd1cb07e6f3d89dccdf3a7a77989b8
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
    "id": 47,
    "updated_at": "2016-12-08T18:27:07.671Z",
    "course_id": 108,
    "author_id": 251,
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
curl "api.goskive.com/v2/chapters/47" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c08b6a9aa97a356e921d870de7975e61f8dd1cb07e6f3d89dccdf3a7a77989b8"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/9
Content-Type: application/json
Authorization: Bearer 02369a0bf34b727076a64c12d559b65f4487de43c69f20004216a9b388271b1c
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02369a0bf34b727076a64c12d559b65f4487de43c69f20004216a9b388271b1c"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c5004169e058ed5319ac15b2a25f3bd5350ab67f29d3925c2541cedb52182165
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
      "author_id": 326,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:12.649Z",
      "status": "published",
      "subject_id": 133,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 328,
      "reply_to_id": 26,
      "created_at": "2016-12-08T18:27:12.761Z",
      "status": "published",
      "subject_id": 134,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 330,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:12.878Z",
      "status": "published",
      "subject_id": 135,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 332,
      "reply_to_id": 28,
      "created_at": "2016-12-08T18:27:12.998Z",
      "status": "published",
      "subject_id": 136,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 334,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:13.115Z",
      "status": "reported",
      "subject_id": 137,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 336,
      "reply_to_id": 30,
      "created_at": "2016-12-08T18:27:13.227Z",
      "status": "published",
      "subject_id": 138,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 338,
      "reply_to_id": 30,
      "created_at": "2016-12-08T18:27:13.345Z",
      "status": "published",
      "subject_id": 139,
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
	-H "Authorization: Bearer c5004169e058ed5319ac15b2a25f3bd5350ab67f29d3925c2541cedb52182165"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e27c580b76876f66b19d120fb9bbc421eb0fe2ad5bfaa537d313f27ee3f20c66
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
      "id": 40,
      "author_id": 356,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:14.592Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 358,
      "reply_to_id": 40,
      "created_at": "2016-12-08T18:27:14.696Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 360,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:14.802Z",
      "status": "published",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 362,
      "reply_to_id": 42,
      "created_at": "2016-12-08T18:27:14.905Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 364,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:15.011Z",
      "status": "reported",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 366,
      "reply_to_id": 44,
      "created_at": "2016-12-08T18:27:15.115Z",
      "status": "published",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 368,
      "reply_to_id": 44,
      "created_at": "2016-12-08T18:27:15.220Z",
      "status": "published",
      "subject_id": 153,
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
	-H "Authorization: Bearer e27c580b76876f66b19d120fb9bbc421eb0fe2ad5bfaa537d313f27ee3f20c66"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer f49a83f642a28a5f21c6192c5f064bb401de3c161d9ffcde4d970ffc5c2b016d
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
      "author_id": 343,
      "reply_to_id": 33,
      "created_at": "2016-12-08T18:27:13.642Z",
      "status": "published",
      "subject_id": 141,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 347,
      "reply_to_id": 35,
      "created_at": "2016-12-08T18:27:13.871Z",
      "status": "published",
      "subject_id": 143,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 351,
      "reply_to_id": 37,
      "created_at": "2016-12-08T18:27:14.098Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 353,
      "reply_to_id": 37,
      "created_at": "2016-12-08T18:27:14.217Z",
      "status": "published",
      "subject_id": 146,
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
	-H "Authorization: Bearer f49a83f642a28a5f21c6192c5f064bb401de3c161d9ffcde4d970ffc5c2b016d"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 6c4ccd3c2fbd64c06349d84be5d4ccf487121f2908f3d29b45a9a363d6e63570
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
      "author_id": 304,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:11.433Z",
      "status": "reported",
      "subject_id": 123,
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
	-H "Authorization: Bearer 6c4ccd3c2fbd64c06349d84be5d4ccf487121f2908f3d29b45a9a363d6e63570"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/48/republish
Content-Type: application/json
Authorization: Bearer 0a1e1e01accd3453dac50b604c2a89f18005bbea338276ac1c58f6b99418e58e
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
	-H "Authorization: Bearer 0a1e1e01accd3453dac50b604c2a89f18005bbea338276ac1c58f6b99418e58e"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fd66d5cc93db85fd59cb5d2abd223fb7570a56a94d8c957533dba852a4ef605e
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
    "id": 194,
    "updated_at": "2016-12-08T18:28:02.947Z",
    "course_id": 315,
    "author_id": 980,
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
	-H "Authorization: Bearer fd66d5cc93db85fd59cb5d2abd223fb7570a56a94d8c957533dba852a4ef605e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/316/chapters
Content-Type: application/json
Authorization: Bearer 9744ee0632cfd4f222fba48b06dece29102a4032a90401f64c52ba59c8f43b6a
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
    "id": 195,
    "updated_at": "2016-12-08T18:28:03.113Z",
    "course_id": 316,
    "author_id": 982,
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
curl "api.goskive.com/v2/courses/316/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9744ee0632cfd4f222fba48b06dece29102a4032a90401f64c52ba59c8f43b6a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c139fe112011337d35a6e81a3a1f885b4616e6c7bdf335a49decceba551580fd
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
      "id": 175,
      "updated_at": "2016-12-08T18:28:00.263Z",
      "course_id": 304,
      "author_id": 937,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 154",
      "position": 1
    },
    {
      "id": 176,
      "updated_at": "2016-12-08T18:28:00.287Z",
      "course_id": 304,
      "author_id": 938,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 155",
      "position": 2
    },
    {
      "id": 177,
      "updated_at": "2016-12-08T18:28:00.503Z",
      "course_id": 304,
      "author_id": 939,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-08T18:28:00.161Z",
      "questions_updated_at": "2016-12-08T18:28:00.161Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 156",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c139fe112011337d35a6e81a3a1f885b4616e6c7bdf335a49decceba551580fd"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3069d3498f10645d22626050d7932ae58701b9466a6c3b85c414d4e188192167
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
      "id": 178,
      "updated_at": "2016-12-08T18:28:00.820Z",
      "course_id": 306,
      "author_id": 946,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 157",
      "position": 1
    },
    {
      "id": 179,
      "updated_at": "2016-12-08T18:28:00.845Z",
      "course_id": 306,
      "author_id": 947,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 158",
      "position": 2
    },
    {
      "id": 180,
      "updated_at": "2016-12-08T18:28:00.870Z",
      "course_id": 306,
      "author_id": 948,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 159",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3069d3498f10645d22626050d7932ae58701b9466a6c3b85c414d4e188192167"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/4
Content-Type: application/json
Authorization: Bearer ca9328abc2bfb4c05a3a2f5547b7546144c465fc085f61e742b6bfd39a3707ca
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca9328abc2bfb4c05a3a2f5547b7546144c465fc085f61e742b6bfd39a3707ca"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 61a33a7ca8b5c188cf703327cfd29a322fccd0c4cbf039ae8ad654cb6647172b
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
	-H "Authorization: Bearer 61a33a7ca8b5c188cf703327cfd29a322fccd0c4cbf039ae8ad654cb6647172b"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4c869c97389e9cc75889bc71449ee13b55b8a7ea6bd25c4255c125a0a51f2cd8
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
    "creator_id": 51,
    "id": 16,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 16,
    "additional_university_ids": [

    ],
    "discipline_id": 21,
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
    "chapters_updated_at": "2016-12-08T18:26:44.764Z",
    "updated_at": "2016-12-08T18:26:46.003Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 51,
        "chapter_id": 12,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.782Z",
        "created_at": "2016-12-08T18:26:45.782Z",
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
        "author_id": 51,
        "chapter_id": 13,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.858Z",
        "created_at": "2016-12-08T18:26:45.858Z",
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
        "author_id": 51,
        "chapter_id": 12,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.825Z",
        "created_at": "2016-12-08T18:26:45.825Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 51,
        "chapter_id": 13,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.901Z",
        "created_at": "2016-12-08T18:26:45.901Z",
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
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 54,
        "chapter_id": 12,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.941Z",
        "created_at": "2016-12-08T18:26:45.941Z",
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
        "author_id": 55,
        "chapter_id": 13,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:45.982Z",
        "created_at": "2016-12-08T18:26:45.982Z",
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
        "id": 12,
        "updated_at": "2016-12-08T18:26:45.952Z",
        "course_id": 16,
        "author_id": 51,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T18:26:44.764Z",
        "questions_updated_at": "2016-12-08T18:26:44.764Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 12",
        "position": 1
      },
      {
        "id": 13,
        "updated_at": "2016-12-08T18:26:45.992Z",
        "course_id": 16,
        "author_id": 51,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T18:26:44.764Z",
        "questions_updated_at": "2016-12-08T18:26:44.764Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 13",
        "position": 2
      }
    ],
    "topic_id": 21,
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
	-H "Authorization: Bearer 4c869c97389e9cc75889bc71449ee13b55b8a7ea6bd25c4255c125a0a51f2cd8"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/21
Content-Type: application/json
Authorization: Bearer 87213fdc762fa61677aa1f87aef52348c72b8ee136d917a7840e61145f188768
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
    "creator_id": 68,
    "id": 21,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 21,
    "additional_university_ids": [

    ],
    "discipline_id": 26,
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
    "updated_at": "2016-12-08T18:26:48.187Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 26,
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
curl "api.goskive.com/v2/courses/21" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87213fdc762fa61677aa1f87aef52348c72b8ee136d917a7840e61145f188768"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6d2edfa1f9abe72bbabd7afc6c566b9269fbf0a639612efb5d276f2f6c0932c5
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
    "creator_id": 66,
    "id": 20,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 20,
    "additional_university_ids": [

    ],
    "discipline_id": 25,
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
    "updated_at": "2016-12-08T18:26:48.016Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 25,
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
	-H "Authorization: Bearer 6d2edfa1f9abe72bbabd7afc6c566b9269fbf0a639612efb5d276f2f6c0932c5"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 8185cb2d157e92762e82b1f574485a482e5d76cca63785bbdf8dd3c96afb93de
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
      "user_id": 706,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:41.877Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 710,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:42.148Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 714,
      "feedbackable_id": 101,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:42.420Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 718,
      "feedbackable_id": 102,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:42.693Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 37,
      "user_id": 722,
      "feedbackable_id": 103,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T18:27:42.967Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8185cb2d157e92762e82b1f574485a482e5d76cca63785bbdf8dd3c96afb93de"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer a4ec88997490fd4c468df855b8954c19aec6306ecf934b2ef2e0368cce58aff6
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
      "user_id": 701,
      "feedbackable_id": 98,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T18:27:41.542Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4ec88997490fd4c468df855b8954c19aec6306ecf934b2ef2e0368cce58aff6"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 737afd4b82144fae89bd8335738bb697b5cf66c363c726d5a3ccb026e9ac3845
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 737afd4b82144fae89bd8335738bb697b5cf66c363c726d5a3ccb026e9ac3845"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/16/metadata
Content-Type: application/json
Authorization: Bearer a6b0c333359d44e3c151abc7f71bf4343bdbe7ddc0395deb6e6553adaa9d4d6a
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
    "id": 16,
    "uploader": {
      "id": 790,
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
      "created_at": "2016-12-08T18:27:46.764Z",
      "updated_at": "2016-12-08T18:27:46.764Z"
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
    "created_at": "2016-12-08T18:27:46.864Z",
    "updated_at": "2016-12-08T18:27:46.864Z",
    "course_id": 261,
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
curl "api.goskive.com/v2/files/16/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6b0c333359d44e3c151abc7f71bf4343bdbe7ddc0395deb6e6553adaa9d4d6a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/70/feedbacks
Content-Type: application/json
Authorization: Bearer d7debdb43d674265380c3bce3e8d03acab4f5fe3665f14b05204baad6329a3d0
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
      "id": 14,
      "user_id": 580,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:31.748Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 579,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:31.738Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/70/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7debdb43d674265380c3bce3e8d03acab4f5fe3665f14b05204baad6329a3d0"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5153a0101c0477339b9a4a46cedb5b441126bf098ab2d106ffeeda2d445e0543
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 406,
      "chapter_id": 63,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:17.907Z",
      "created_at": "2016-12-08T18:27:17.907Z",
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
      "author_id": 409,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:18.073Z",
      "created_at": "2016-12-08T18:27:18.073Z",
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
      "author_id": 412,
      "chapter_id": 65,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:18.238Z",
      "created_at": "2016-12-08T18:27:18.238Z",
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
      "id": 48,
      "obfuscated_id": "oqXJ8Hi_AE4",
      "author_id": 415,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:18.402Z",
      "created_at": "2016-12-08T18:27:18.402Z",
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 418,
      "chapter_id": 67,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:18.567Z",
      "created_at": "2016-12-08T18:27:18.567Z",
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
	-H "Authorization: Bearer 5153a0101c0477339b9a4a46cedb5b441126bf098ab2d106ffeeda2d445e0543"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4c952e9b342221b1749fec54547faab90c174ca1196ec5894281676f3d90561b
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 434,
      "chapter_id": 72,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:19.478Z",
      "created_at": "2016-12-08T18:27:19.478Z",
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
	-H "Authorization: Bearer 4c952e9b342221b1749fec54547faab90c174ca1196ec5894281676f3d90561b"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/republish
Content-Type: application/json
Authorization: Bearer 3a8de662d7647b4490e6dcffb99424fd7359af5ce35a1c388663e3c97e4fae59
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a8de662d7647b4490e6dcffb99424fd7359af5ce35a1c388663e3c97e4fae59"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/62/feedbacks
Content-Type: application/json
Authorization: Bearer 261990c533a11e9b2827a4c70d1942277fb5a15ff2398f8d91f1b1d7ba104a1b
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
      "id": 3,
      "user_id": 464,
      "feedbackable_id": 62,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:21.314Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 463,
      "feedbackable_id": 62,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:21.302Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/62/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 261990c533a11e9b2827a4c70d1942277fb5a15ff2398f8d91f1b1d7ba104a1b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 5c916758078d5653930b6d7297189fcbd0353312bc904e6a6cfc676f305bd16d
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
      "id": 116,
      "obfuscated_id": "PhHGVKqnHFA",
      "author_id": 874,
      "chapter_id": 156,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:54.519Z",
      "created_at": "2016-12-08T18:27:54.436Z",
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
      "author_id": 877,
      "chapter_id": 157,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:54.781Z",
      "created_at": "2016-12-08T18:27:54.698Z",
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
    },
    {
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 880,
      "chapter_id": 158,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:55.043Z",
      "created_at": "2016-12-08T18:27:54.960Z",
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
          "id": 238,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 239,
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
      "author_id": 883,
      "chapter_id": 159,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:55.307Z",
      "created_at": "2016-12-08T18:27:55.223Z",
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
          "id": 240,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 241,
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
      "author_id": 886,
      "chapter_id": 160,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:55.564Z",
      "created_at": "2016-12-08T18:27:55.486Z",
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
          "id": 242,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 243,
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
	-H "Authorization: Bearer 5c916758078d5653930b6d7297189fcbd0353312bc904e6a6cfc676f305bd16d"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 19ca03bf3f6ae6d1b25820bead89a49587a8fe3ea563dd9c71bca2993ffd3a81
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
      "author_id": 902,
      "chapter_id": 165,
      "position": 118,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:56.948Z",
      "created_at": "2016-12-08T18:27:56.870Z",
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
          "id": 252,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 253,
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
	-H "Authorization: Bearer 19ca03bf3f6ae6d1b25820bead89a49587a8fe3ea563dd9c71bca2993ffd3a81"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/110/republish
Content-Type: application/json
Authorization: Bearer ca2999f33d09661603228b2d9dc3563eff44e6d8d8c9c2aada1ea78efc0c561e
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca2999f33d09661603228b2d9dc3563eff44e6d8d8c9c2aada1ea78efc0c561e"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 15a282bceb0821dc91ac9f0bf966dd1e45f72aa2ee1043cf49e25909f90b1f47
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":76,"published":false}}
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
    "creator_id": 200,
    "id": 69,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 70,
    "additional_university_ids": [

    ],
    "discipline_id": 77,
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
    "updated_at": "2016-12-08T18:27:02.807Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 76,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":76,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15a282bceb0821dc91ac9f0bf966dd1e45f72aa2ee1043cf49e25909f90b1f47"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7efb3814ce4f9e3e17cc2304a8dd4217522240929b9b9e52e22c95b12d7295b3
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
      "creator_id": 228,
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-61",
      "html_url": "https://goskive.com/course/fu-course-61",
      "slug": "fu-course-61",
      "university_id": 80,
      "additional_university_ids": [

      ],
      "discipline_id": 102,
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
      "updated_at": "2016-12-08T18:27:05.518Z",
      "shortname": "fu-course-61",
      "topic_id": 101,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 228,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-62",
      "html_url": "https://goskive.com/course/fu-course-62",
      "slug": "fu-course-62",
      "university_id": 80,
      "additional_university_ids": [

      ],
      "discipline_id": 103,
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
      "updated_at": "2016-12-08T18:27:05.551Z",
      "shortname": "fu-course-62",
      "topic_id": 102,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 62",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 229,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-63",
      "html_url": "https://goskive.com/course/fu-course-63",
      "slug": "fu-course-63",
      "university_id": 80,
      "additional_university_ids": [

      ],
      "discipline_id": 104,
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
      "updated_at": "2016-12-08T18:27:05.593Z",
      "shortname": "fu-course-63",
      "topic_id": 103,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 63",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 229,
      "id": 97,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-64",
      "html_url": "https://goskive.com/course/fu-course-64",
      "slug": "fu-course-64",
      "university_id": 80,
      "additional_university_ids": [

      ],
      "discipline_id": 105,
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
      "chapters_updated_at": "2016-12-08T18:27:05.437Z",
      "updated_at": "2016-12-08T18:27:05.873Z",
      "shortname": "fu-course-64",
      "topic_id": 104,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 64",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7efb3814ce4f9e3e17cc2304a8dd4217522240929b9b9e52e22c95b12d7295b3"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ce184b40c4fa91a55f886af3b31efc496c7c4d59462d0913b23faa3cb5860aed
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
      "creator_id": 234,
      "id": 98,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-65",
      "html_url": "https://goskive.com/course/fu-course-65",
      "slug": "fu-course-65",
      "university_id": 81,
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
      "updated_at": "2016-12-08T18:27:06.059Z",
      "shortname": "fu-course-65",
      "topic_id": 105,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 65",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 234,
      "id": 99,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-66",
      "html_url": "https://goskive.com/course/fu-course-66",
      "slug": "fu-course-66",
      "university_id": 81,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-12-08T18:27:06.093Z",
      "shortname": "fu-course-66",
      "topic_id": 106,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 66",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 235,
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-67",
      "html_url": "https://goskive.com/course/fu-course-67",
      "slug": "fu-course-67",
      "university_id": 81,
      "additional_university_ids": [

      ],
      "discipline_id": 108,
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
      "updated_at": "2016-12-08T18:27:06.137Z",
      "shortname": "fu-course-67",
      "topic_id": 107,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 235,
      "id": 101,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-68",
      "html_url": "https://goskive.com/course/fu-course-68",
      "slug": "fu-course-68",
      "university_id": 81,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-12-08T18:27:06.170Z",
      "shortname": "fu-course-68",
      "topic_id": 108,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce184b40c4fa91a55f886af3b31efc496c7c4d59462d0913b23faa3cb5860aed"
```
