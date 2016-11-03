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
DELETE /v2/chapters/170
Content-Type: application/json
Authorization: Bearer 2e6a72e0bcc1fc67e26f4c0eddcbbdf2ef1d7f8bcc5c6af34e34d5f580bd1b70
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/170" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e6a72e0bcc1fc67e26f4c0eddcbbdf2ef1d7f8bcc5c6af34e34d5f580bd1b70"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/168
Content-Type: application/json
Authorization: Bearer 0af44fa6af77a1ccd1fd51ac9d0f1a72414646380b673e2cbd2b0f49313cb792
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
    "id": 168,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T17:48:47.027Z",
    "course_id": 266,
    "author_id": 829,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-03T17:48:46.464Z",
    "questions_updated_at": "2016-11-03T17:48:46.464Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 66,
        "obfuscated_id": "H7dODBospvw",
        "author_id": 832,
        "chapter_id": 168,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:46.967Z",
        "created_at": "2016-11-03T17:48:46.967Z",
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
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 833,
        "chapter_id": 168,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:47.009Z",
        "created_at": "2016-11-03T17:48:47.009Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 830,
        "chapter_id": 168,
        "position": 80,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:46.691Z",
        "created_at": "2016-11-03T17:48:46.576Z",
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
            "id": 189,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 190,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 94,
        "obfuscated_id": "CVi6VU_nV6k",
        "author_id": 831,
        "chapter_id": 168,
        "position": 81,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:46.893Z",
        "created_at": "2016-11-03T17:48:46.767Z",
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
            "id": 191,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 192,
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
curl "api.goskive.com/v2/chapters/168" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0af44fa6af77a1ccd1fd51ac9d0f1a72414646380b673e2cbd2b0f49313cb792"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/166
Content-Type: application/json
Authorization: Bearer 7415d8fc7e2bb48b6000ea1b4e99f63ac427aab054ddeaff15a5c93a14bcdb21
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
    "id": 166,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T17:48:46.299Z",
    "course_id": 264,
    "author_id": 823,
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
curl "api.goskive.com/v2/chapters/166" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7415d8fc7e2bb48b6000ea1b4e99f63ac427aab054ddeaff15a5c93a14bcdb21"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 12a45b2b514ae9094f49a9c292c11c3802e2d0adab4725369a6316e36e85f334
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12a45b2b514ae9094f49a9c292c11c3802e2d0adab4725369a6316e36e85f334"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 630c875c4c351ce78d5a0ad5e692e3c43967a6d82a3a38b1543349b5e94df810
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
      "id": 16,
      "author_id": 264,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:56.750Z",
      "status": "published",
      "subject_id": 79,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 266,
      "reply_to_id": 16,
      "created_at": "2016-11-03T17:47:56.839Z",
      "status": "published",
      "subject_id": 80,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 268,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:56.928Z",
      "status": "published",
      "subject_id": 81,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 270,
      "reply_to_id": 18,
      "created_at": "2016-11-03T17:47:57.015Z",
      "status": "published",
      "subject_id": 82,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 272,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:57.102Z",
      "status": "reported",
      "subject_id": 83,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 274,
      "reply_to_id": 20,
      "created_at": "2016-11-03T17:47:57.188Z",
      "status": "published",
      "subject_id": 84,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 276,
      "reply_to_id": 20,
      "created_at": "2016-11-03T17:47:57.274Z",
      "status": "published",
      "subject_id": 85,
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
	-H "Authorization: Bearer 630c875c4c351ce78d5a0ad5e692e3c43967a6d82a3a38b1543349b5e94df810"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 271bd51c6186f4e4b412ee689effc06863dd38d04f9e0cfcc4f87b10d460cbb2
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
      "id": 37,
      "author_id": 309,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:58.754Z",
      "status": "published",
      "subject_id": 100,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 311,
      "reply_to_id": 37,
      "created_at": "2016-11-03T17:47:58.840Z",
      "status": "published",
      "subject_id": 101,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 313,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:58.929Z",
      "status": "published",
      "subject_id": 102,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 315,
      "reply_to_id": 39,
      "created_at": "2016-11-03T17:47:59.016Z",
      "status": "published",
      "subject_id": 103,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 317,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:59.106Z",
      "status": "reported",
      "subject_id": 104,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 319,
      "reply_to_id": 41,
      "created_at": "2016-11-03T17:47:59.194Z",
      "status": "published",
      "subject_id": 105,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 321,
      "reply_to_id": 41,
      "created_at": "2016-11-03T17:47:59.284Z",
      "status": "published",
      "subject_id": 106,
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
	-H "Authorization: Bearer 271bd51c6186f4e4b412ee689effc06863dd38d04f9e0cfcc4f87b10d460cbb2"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 6ba6997c0935bef9682b4f9d43a11148406b9c76da053c4ab1352e28c398ea0f
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
      "id": 10,
      "author_id": 251,
      "reply_to_id": 9,
      "created_at": "2016-11-03T17:47:56.149Z",
      "status": "published",
      "subject_id": 73,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 255,
      "reply_to_id": 11,
      "created_at": "2016-11-03T17:47:56.329Z",
      "status": "published",
      "subject_id": 75,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 259,
      "reply_to_id": 13,
      "created_at": "2016-11-03T17:47:56.498Z",
      "status": "published",
      "subject_id": 77,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 261,
      "reply_to_id": 13,
      "created_at": "2016-11-03T17:47:56.611Z",
      "status": "published",
      "subject_id": 78,
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
	-H "Authorization: Bearer 6ba6997c0935bef9682b4f9d43a11148406b9c76da053c4ab1352e28c398ea0f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 8733a4e9204bb42a50b9cff43f72dcd58c26ff0d7fe7c6879413678e80e93825
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
      "id": 34,
      "author_id": 302,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:47:58.444Z",
      "status": "reported",
      "subject_id": 97,
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
	-H "Authorization: Bearer 8733a4e9204bb42a50b9cff43f72dcd58c26ff0d7fe7c6879413678e80e93825"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer c9bc8085a6e122865369c5679f763f814a337eb7b5b99a3fef7a4cc2dc7278f9
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
	-H "Authorization: Bearer c9bc8085a6e122865369c5679f763f814a337eb7b5b99a3fef7a4cc2dc7278f9"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/19/chapters
Content-Type: application/json
Authorization: Bearer 5163375b05671f35de85bf01749b4a6fd22ad9b8309f66e59bb6245eeab5ac25
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
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T17:47:43.429Z",
    "course_id": 19,
    "author_id": 66,
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
curl "api.goskive.com/v2/courses/19/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5163375b05671f35de85bf01749b4a6fd22ad9b8309f66e59bb6245eeab5ac25"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1988c94a51b3017178de1487d99807ba1c7aa6ba0f66d2f60bcf90b0f187d5e4
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
    "id": 24,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T17:47:43.871Z",
    "course_id": 22,
    "author_id": 72,
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
	-H "Authorization: Bearer 1988c94a51b3017178de1487d99807ba1c7aa6ba0f66d2f60bcf90b0f187d5e4"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 22c37e2670cda0b07353de76db58f7f2eeb2236dedb8dc196d000560259051e4
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
      "id": 10,
      "title": "Clever Chapter Title 10",
      "position": 1,
      "updated_at": "2016-11-03T17:47:41.994Z",
      "course_id": 13,
      "author_id": 41,
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
      "id": 11,
      "title": "Clever Chapter Title 11",
      "position": 2,
      "updated_at": "2016-11-03T17:47:42.019Z",
      "course_id": 13,
      "author_id": 42,
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
      "id": 12,
      "title": "Clever Chapter Title 12",
      "position": 3,
      "updated_at": "2016-11-03T17:47:42.283Z",
      "course_id": 13,
      "author_id": 43,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-03T17:47:41.917Z",
      "questions_updated_at": "2016-11-03T17:47:41.917Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22c37e2670cda0b07353de76db58f7f2eeb2236dedb8dc196d000560259051e4"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3bf5b8e0bca485c8418db52e74e79938204a9a77fc47a802f6cc92402c1e8cbd
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
      "id": 13,
      "title": "Clever Chapter Title 13",
      "position": 1,
      "updated_at": "2016-11-03T17:47:42.531Z",
      "course_id": 15,
      "author_id": 50,
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
      "id": 14,
      "title": "Clever Chapter Title 14",
      "position": 2,
      "updated_at": "2016-11-03T17:47:42.555Z",
      "course_id": 15,
      "author_id": 51,
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
      "id": 15,
      "title": "Clever Chapter Title 15",
      "position": 3,
      "updated_at": "2016-11-03T17:47:42.580Z",
      "course_id": 15,
      "author_id": 52,
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
	-H "Authorization: Bearer 3bf5b8e0bca485c8418db52e74e79938204a9a77fc47a802f6cc92402c1e8cbd"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 100769f692574a4647d4db566a4dec863ab300503df52b79e51f15750d1fc737
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
	-H "Authorization: Bearer 100769f692574a4647d4db566a4dec863ab300503df52b79e51f15750d1fc737"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/307
Content-Type: application/json
Authorization: Bearer 95a06d600fdea5779480cd2dab42b6a532f0b83290447bb813007c73a43ad2dd
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/307" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95a06d600fdea5779480cd2dab42b6a532f0b83290447bb813007c73a43ad2dd"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer dfd73813d5a996c914c38247d362ce45882c76795420472813536192f5bc0a77
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
    "creator_id": 959,
    "id": 311,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 296,
    "additional_university_ids": [

    ],
    "topic_id": 323,
    "discipline_id": 324,
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
    "chapters_updated_at": "2016-11-03T17:48:59.255Z",
    "updated_at": "2016-11-03T17:49:00.788Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 188,
        "title": "Clever Chapter Title 164",
        "position": 1,
        "updated_at": "2016-11-03T17:49:00.738Z",
        "course_id": 311,
        "author_id": 959,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T17:48:59.255Z",
        "questions_updated_at": "2016-11-03T17:48:59.255Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 189,
        "title": "Clever Chapter Title 165",
        "position": 2,
        "updated_at": "2016-11-03T17:49:00.779Z",
        "course_id": 311,
        "author_id": 959,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T17:48:59.255Z",
        "questions_updated_at": "2016-11-03T17:48:59.255Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 959,
        "chapter_id": 188,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.568Z",
        "created_at": "2016-11-03T17:49:00.568Z",
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
        "author_id": 959,
        "chapter_id": 189,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.643Z",
        "created_at": "2016-11-03T17:49:00.643Z",
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
        "author_id": 959,
        "chapter_id": 188,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.610Z",
        "created_at": "2016-11-03T17:49:00.610Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 959,
        "chapter_id": 189,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.686Z",
        "created_at": "2016-11-03T17:49:00.686Z",
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
        "author_id": 962,
        "chapter_id": 188,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.728Z",
        "created_at": "2016-11-03T17:49:00.728Z",
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
        "author_id": 963,
        "chapter_id": 189,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:00.769Z",
        "created_at": "2016-11-03T17:49:00.769Z",
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
	-H "Authorization: Bearer dfd73813d5a996c914c38247d362ce45882c76795420472813536192f5bc0a77"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/297
Content-Type: application/json
Authorization: Bearer 57d63971851526020517e29b85c32319fafcca70232b9504c6a82a5ad3c33520
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
    "creator_id": 922,
    "id": 297,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 282,
    "additional_university_ids": [

    ],
    "topic_id": 309,
    "discipline_id": 310,
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
    "updated_at": "2016-11-03T17:48:54.190Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/297" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57d63971851526020517e29b85c32319fafcca70232b9504c6a82a5ad3c33520"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e131e6b0a06135095913eeea9da1f269acf260745085e6037d9bc90fd5b441dd
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
    "creator_id": 920,
    "id": 296,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 281,
    "additional_university_ids": [

    ],
    "topic_id": 308,
    "discipline_id": 309,
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
    "updated_at": "2016-11-03T17:48:54.044Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e131e6b0a06135095913eeea9da1f269acf260745085e6037d9bc90fd5b441dd"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer eca71132f7491200c33f9ff86d52cf278858c881c72f5b30d329ec9104845d85
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
      "id": 31,
      "user_id": 730,
      "feedbackable_id": 75,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:37.822Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 734,
      "feedbackable_id": 76,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:38.133Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 738,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:38.453Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 742,
      "feedbackable_id": 78,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:38.776Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 746,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T17:48:39.115Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eca71132f7491200c33f9ff86d52cf278858c881c72f5b30d329ec9104845d85"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 4e32fc16d860727e88f302e7f84dd757a05733470aafb220ebf8e6d26a921fbd
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
      "id": 21,
      "user_id": 688,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T17:48:34.524Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e32fc16d860727e88f302e7f84dd757a05733470aafb220ebf8e6d26a921fbd"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 90a2211377ca6ef09036ea18373f1acab47282e0dd43dc66872e26cbb1b6cf63
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90a2211377ca6ef09036ea18373f1acab47282e0dd43dc66872e26cbb1b6cf63"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer c209c3e1ba1a9ea53c61a4c4ecac0e4735959d4d28b9c65b993c2843fe2029a8
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
      "id": 545,
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
      "created_at": "2016-11-03T17:48:24.419Z",
      "updated_at": "2016-11-03T17:48:24.419Z"
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
    "created_at": "2016-11-03T17:48:24.498Z",
    "updated_at": "2016-11-03T17:48:24.498Z",
    "course_id": 195,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c209c3e1ba1a9ea53c61a4c4ecac0e4735959d4d28b9c65b993c2843fe2029a8"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/8/feedbacks
Content-Type: application/json
Authorization: Bearer e87f0c48d7cb0fbb30d57f5f8e7ac62553cd458d396cbe6e02cba9c8ed1bf28c
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
      "user_id": 103,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:47:46.950Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 102,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:47:46.938Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e87f0c48d7cb0fbb30d57f5f8e7ac62553cd458d396cbe6e02cba9c8ed1bf28c"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer e52194f32c6aacdd5ceaeb6395bc3136abe1af9c66db2c9e07e52b65e62f27da
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 162,
      "chapter_id": 44,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:50.764Z",
      "created_at": "2016-11-03T17:47:50.764Z",
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 165,
      "chapter_id": 45,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:50.924Z",
      "created_at": "2016-11-03T17:47:50.924Z",
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
      "author_id": 168,
      "chapter_id": 46,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:51.074Z",
      "created_at": "2016-11-03T17:47:51.074Z",
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
      "author_id": 171,
      "chapter_id": 47,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:51.221Z",
      "created_at": "2016-11-03T17:47:51.221Z",
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 174,
      "chapter_id": 48,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:51.363Z",
      "created_at": "2016-11-03T17:47:51.363Z",
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
	-H "Authorization: Bearer e52194f32c6aacdd5ceaeb6395bc3136abe1af9c66db2c9e07e52b65e62f27da"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 2878a9c377e7e51b9dd2e74cfb54b55713a6228f47a4ed581783381f44f79441
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 206,
      "chapter_id": 58,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:52.988Z",
      "created_at": "2016-11-03T17:47:52.988Z",
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
	-H "Authorization: Bearer 2878a9c377e7e51b9dd2e74cfb54b55713a6228f47a4ed581783381f44f79441"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/18/republish
Content-Type: application/json
Authorization: Bearer 03bb86c5978d217464b295e37de13e60acc6a60af433f8d4efced03e8278f9f1
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/18/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03bb86c5978d217464b295e37de13e60acc6a60af433f8d4efced03e8278f9f1"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/90/feedbacks
Content-Type: application/json
Authorization: Bearer 133572ab593fd9d2599cde6837caab8147f7a2dd894d343d2f90de3a26ee0a1f
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
      "id": 44,
      "user_id": 813,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:44.992Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 812,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:44.982Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/90/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 133572ab593fd9d2599cde6837caab8147f7a2dd894d343d2f90de3a26ee0a1f"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 686d93676ad742e4a8d8a9dbdccbe175a32437caef9da78e5460742ebe652263
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 517,
      "chapter_id": 106,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:21.816Z",
      "created_at": "2016-11-03T17:48:21.689Z",
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
    },
    {
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 508,
      "chapter_id": 103,
      "position": 36,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:20.922Z",
      "created_at": "2016-11-03T17:48:20.799Z",
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
      "author_id": 511,
      "chapter_id": 104,
      "position": 37,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:21.220Z",
      "created_at": "2016-11-03T17:48:21.093Z",
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 514,
      "chapter_id": 105,
      "position": 38,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:21.519Z",
      "created_at": "2016-11-03T17:48:21.393Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 520,
      "chapter_id": 107,
      "position": 40,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:22.119Z",
      "created_at": "2016-11-03T17:48:21.997Z",
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
          "id": 105,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 106,
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
	-H "Authorization: Bearer 686d93676ad742e4a8d8a9dbdccbe175a32437caef9da78e5460742ebe652263"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 4f6e86c856472d83899d47eba188f326352b7ad00bbe5b92865c5d8fd01a88bd
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
      "id": 46,
      "obfuscated_id": "urkHiAaH08E",
      "author_id": 504,
      "chapter_id": 102,
      "position": 35,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:20.581Z",
      "created_at": "2016-11-03T17:48:20.460Z",
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
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f6e86c856472d83899d47eba188f326352b7ad00bbe5b92865c5d8fd01a88bd"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/52/republish
Content-Type: application/json
Authorization: Bearer 99caa629cad53a929b6886623b9a4741f725ea058747c6f07175bd3dca151835
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99caa629cad53a929b6886623b9a4741f725ea058747c6f07175bd3dca151835"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 39329380df47d54307c7975f18646192abb7b559290e611d42b81c7a92c50809
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":157,"published":false}}
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
    "creator_id": 420,
    "id": 155,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 138,
    "additional_university_ids": [

    ],
    "topic_id": 157,
    "discipline_id": 158,
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
    "updated_at": "2016-11-03T17:48:11.846Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":157,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39329380df47d54307c7975f18646192abb7b559290e611d42b81c7a92c50809"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4fd65ff766dbe42cff3020de3b54ded9927d32114d5bce4ea7d5cbfc419aa390
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
      "creator_id": 400,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 141,
      "discipline_id": 142,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
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
      "updated_at": "2016-11-03T17:48:09.936Z",
      "shortname": "fu-course-102"
    },
    {
      "creator_id": 400,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 142,
      "discipline_id": 143,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
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
      "updated_at": "2016-11-03T17:48:09.979Z",
      "shortname": "fu-course-103"
    },
    {
      "creator_id": 401,
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-104",
      "html_url": "https://goskive.com/course/fu-course-104",
      "slug": "fu-course-104",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 143,
      "discipline_id": 144,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
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
      "updated_at": "2016-11-03T17:48:10.030Z",
      "shortname": "fu-course-104"
    },
    {
      "creator_id": 401,
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 144,
      "discipline_id": 145,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
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
      "chapters_updated_at": "2016-11-03T17:48:10.375Z",
      "updated_at": "2016-11-03T17:48:10.384Z",
      "shortname": "fu-course-105"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fd65ff766dbe42cff3020de3b54ded9927d32114d5bce4ea7d5cbfc419aa390"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fe6dc26e41d3e031af44ab1ea3d4ab835f1d5b056be63193180a40ff3a93cd8d
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
      "creator_id": 406,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 145,
      "discipline_id": 146,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
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
      "updated_at": "2016-11-03T17:48:10.539Z",
      "shortname": "fu-course-106"
    },
    {
      "creator_id": 406,
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 146,
      "discipline_id": 147,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
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
      "updated_at": "2016-11-03T17:48:10.581Z",
      "shortname": "fu-course-107"
    },
    {
      "creator_id": 407,
      "id": 145,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 147,
      "discipline_id": 148,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
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
      "updated_at": "2016-11-03T17:48:10.632Z",
      "shortname": "fu-course-108"
    },
    {
      "creator_id": 407,
      "id": 146,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 148,
      "discipline_id": 149,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
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
      "updated_at": "2016-11-03T17:48:10.675Z",
      "shortname": "fu-course-109"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe6dc26e41d3e031af44ab1ea3d4ab835f1d5b056be63193180a40ff3a93cd8d"
```
