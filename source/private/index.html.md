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
DELETE /v2/chapters/106
Content-Type: application/json
Authorization: Bearer b8e09c32a69fb4cf5ed37768dff4a5d7ea228f3949ab1bbeca2182fdb1cee977
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/106" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8e09c32a69fb4cf5ed37768dff4a5d7ea228f3949ab1bbeca2182fdb1cee977"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/107
Content-Type: application/json
Authorization: Bearer 163078f75e77bcf06267e7603159f4d51ecd9e26fa2346859fc3ec92633a9ca3
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
    "id": 107,
    "updated_at": "2016-12-08T18:10:13.571Z",
    "course_id": 212,
    "author_id": 606,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-08T18:10:13.077Z",
    "questions_updated_at": "2016-12-08T18:10:13.077Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 609,
        "chapter_id": 107,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:13.511Z",
        "created_at": "2016-12-08T18:10:13.511Z",
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
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 610,
        "chapter_id": 107,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:13.553Z",
        "created_at": "2016-12-08T18:10:13.553Z",
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
        "id": 100,
        "obfuscated_id": "erXmBhoMZFI",
        "author_id": 607,
        "chapter_id": 107,
        "position": 87,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:13.293Z",
        "created_at": "2016-12-08T18:10:13.216Z",
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
            "id": 203,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 204,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 101,
        "obfuscated_id": "PprZyBVq_gc",
        "author_id": 608,
        "chapter_id": 107,
        "position": 88,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:13.446Z",
        "created_at": "2016-12-08T18:10:13.360Z",
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
            "id": 205,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 206,
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
curl "api.goskive.com/v2/chapters/107" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 163078f75e77bcf06267e7603159f4d51ecd9e26fa2346859fc3ec92633a9ca3"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/100
Content-Type: application/json
Authorization: Bearer d719b3d1bfe6fe608b495a16803f759ad042118190211a1df70e1e2b378e7a26
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
    "id": 100,
    "updated_at": "2016-12-08T18:10:11.722Z",
    "course_id": 205,
    "author_id": 586,
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
curl "api.goskive.com/v2/chapters/100" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d719b3d1bfe6fe608b495a16803f759ad042118190211a1df70e1e2b378e7a26"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer e165dfb69f07eb5f5f1fc09bb111f7226fe138d71c9e85fc9d4a509748c4414b
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e165dfb69f07eb5f5f1fc09bb111f7226fe138d71c9e85fc9d4a509748c4414b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer fc0ec08b2450f87789353255766ecae041990fe7e0b1939af82cd565a5c16f7d
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
      "id": 24,
      "author_id": 433,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:56.744Z",
      "status": "published",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 435,
      "reply_to_id": 24,
      "created_at": "2016-12-08T18:09:56.857Z",
      "status": "published",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 437,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:56.970Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 439,
      "reply_to_id": 26,
      "created_at": "2016-12-08T18:09:57.081Z",
      "status": "published",
      "subject_id": 154,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 441,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:57.195Z",
      "status": "reported",
      "subject_id": 155,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 443,
      "reply_to_id": 28,
      "created_at": "2016-12-08T18:09:57.309Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 445,
      "reply_to_id": 28,
      "created_at": "2016-12-08T18:09:57.423Z",
      "status": "published",
      "subject_id": 157,
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
	-H "Authorization: Bearer fc0ec08b2450f87789353255766ecae041990fe7e0b1939af82cd565a5c16f7d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c2f58e5672796cae3a28921f528ba3d776af2ac32ab2694ff34a49c412bfe000
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
      "id": 31,
      "author_id": 448,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:57.600Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 450,
      "reply_to_id": 31,
      "created_at": "2016-12-08T18:09:57.712Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 452,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:57.828Z",
      "status": "published",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 454,
      "reply_to_id": 33,
      "created_at": "2016-12-08T18:09:57.939Z",
      "status": "published",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 456,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:58.049Z",
      "status": "reported",
      "subject_id": 162,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 458,
      "reply_to_id": 35,
      "created_at": "2016-12-08T18:09:58.159Z",
      "status": "published",
      "subject_id": 163,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 460,
      "reply_to_id": 35,
      "created_at": "2016-12-08T18:09:58.270Z",
      "status": "published",
      "subject_id": 164,
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
	-H "Authorization: Bearer c2f58e5672796cae3a28921f528ba3d776af2ac32ab2694ff34a49c412bfe000"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 897e1919d6c42f08bc2430ffe80cc74e7e3684035528074863d5d304ef35c07f
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
      "id": 11,
      "author_id": 405,
      "reply_to_id": 10,
      "created_at": "2016-12-08T18:09:55.174Z",
      "status": "published",
      "subject_id": 138,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 409,
      "reply_to_id": 12,
      "created_at": "2016-12-08T18:09:55.400Z",
      "status": "published",
      "subject_id": 140,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 413,
      "reply_to_id": 14,
      "created_at": "2016-12-08T18:09:55.619Z",
      "status": "published",
      "subject_id": 142,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 415,
      "reply_to_id": 14,
      "created_at": "2016-12-08T18:09:55.763Z",
      "status": "published",
      "subject_id": 143,
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
	-H "Authorization: Bearer 897e1919d6c42f08bc2430ffe80cc74e7e3684035528074863d5d304ef35c07f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer a6d4741bb16da0e5164f16a28689a2ac9cceba526d9ef9383542b909a0e8ddca
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
      "id": 42,
      "author_id": 471,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:58.918Z",
      "status": "reported",
      "subject_id": 169,
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
	-H "Authorization: Bearer a6d4741bb16da0e5164f16a28689a2ac9cceba526d9ef9383542b909a0e8ddca"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/46/republish
Content-Type: application/json
Authorization: Bearer cc37b8efb6e0d56316fc8bbb8966c51f10185a46c7afe357d58181a7c1c1a20c
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc37b8efb6e0d56316fc8bbb8966c51f10185a46c7afe357d58181a7c1c1a20c"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/300/chapters
Content-Type: application/json
Authorization: Bearer 9dcdb3489c4167dc813a4e17d48c3b86165db089b5d5580e0e64086845eadfc9
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
    "updated_at": "2016-12-08T18:10:38.509Z",
    "course_id": 300,
    "author_id": 927,
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
curl "api.goskive.com/v2/courses/300/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9dcdb3489c4167dc813a4e17d48c3b86165db089b5d5580e0e64086845eadfc9"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a08c6bd30b380cb2bfd96050e47e85d1781ff8daa10e1050f6c54a7fc2f5f017
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
    "id": 185,
    "updated_at": "2016-12-08T18:10:38.979Z",
    "course_id": 303,
    "author_id": 933,
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
	-H "Authorization: Bearer a08c6bd30b380cb2bfd96050e47e85d1781ff8daa10e1050f6c54a7fc2f5f017"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 887b1b66c9ceffe853b90655582ebf18fc7364409e7d7fa04d3e99bca43817e4
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
      "id": 174,
      "updated_at": "2016-12-08T18:10:37.259Z",
      "course_id": 295,
      "author_id": 906,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 153",
      "position": 1
    },
    {
      "id": 175,
      "updated_at": "2016-12-08T18:10:37.287Z",
      "course_id": 295,
      "author_id": 907,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 154",
      "position": 2
    },
    {
      "id": 176,
      "updated_at": "2016-12-08T18:10:37.510Z",
      "course_id": 295,
      "author_id": 908,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-08T18:10:37.151Z",
      "questions_updated_at": "2016-12-08T18:10:37.151Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 155",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 887b1b66c9ceffe853b90655582ebf18fc7364409e7d7fa04d3e99bca43817e4"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d315d60a61f7f63a9c44cd1dadf12b5920f6b4dfad0314064b485899cb347b2d
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
      "id": 177,
      "updated_at": "2016-12-08T18:10:37.844Z",
      "course_id": 297,
      "author_id": 915,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 156",
      "position": 1
    },
    {
      "id": 178,
      "updated_at": "2016-12-08T18:10:37.871Z",
      "course_id": 297,
      "author_id": 916,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 157",
      "position": 2
    },
    {
      "id": 179,
      "updated_at": "2016-12-08T18:10:37.898Z",
      "course_id": 297,
      "author_id": 917,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 158",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d315d60a61f7f63a9c44cd1dadf12b5920f6b4dfad0314064b485899cb347b2d"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/190
Content-Type: application/json
Authorization: Bearer 0a28929468f6669dcef8a210ca9caa1f821972d1b1a73f604eecdab4dfe94ca8
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/190" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a28929468f6669dcef8a210ca9caa1f821972d1b1a73f604eecdab4dfe94ca8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 29047cd230319e90252a05f27de11eb11917c4082bed22a7c39c405f640f2b88
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
	-H "Authorization: Bearer 29047cd230319e90252a05f27de11eb11917c4082bed22a7c39c405f640f2b88"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 89f8eb4f625f66eb90e695b9f129ff810a53ad54910bd137d94051d344b63bff
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
    "creator_id": 562,
    "id": 201,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 180,
    "additional_university_ids": [

    ],
    "discipline_id": 208,
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
    "chapters_updated_at": "2016-12-08T18:10:06.244Z",
    "updated_at": "2016-12-08T18:10:07.433Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 562,
        "chapter_id": 92,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.209Z",
        "created_at": "2016-12-08T18:10:07.209Z",
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
        "author_id": 562,
        "chapter_id": 93,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.286Z",
        "created_at": "2016-12-08T18:10:07.286Z",
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
        "author_id": 562,
        "chapter_id": 92,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.252Z",
        "created_at": "2016-12-08T18:10:07.252Z",
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
        "author_id": 562,
        "chapter_id": 93,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.329Z",
        "created_at": "2016-12-08T18:10:07.329Z",
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
        "author_id": 565,
        "chapter_id": 92,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.370Z",
        "created_at": "2016-12-08T18:10:07.370Z",
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
        "author_id": 566,
        "chapter_id": 93,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.412Z",
        "created_at": "2016-12-08T18:10:07.412Z",
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
        "id": 92,
        "updated_at": "2016-12-08T18:10:07.380Z",
        "course_id": 201,
        "author_id": 562,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T18:10:06.244Z",
        "questions_updated_at": "2016-12-08T18:10:06.244Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 83",
        "position": 1
      },
      {
        "id": 93,
        "updated_at": "2016-12-08T18:10:07.423Z",
        "course_id": 201,
        "author_id": 562,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T18:10:06.244Z",
        "questions_updated_at": "2016-12-08T18:10:06.244Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 84",
        "position": 2
      }
    ],
    "topic_id": 208,
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
	-H "Authorization: Bearer 89f8eb4f625f66eb90e695b9f129ff810a53ad54910bd137d94051d344b63bff"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/186
Content-Type: application/json
Authorization: Bearer 816fa7b83a6c6d85286707ad0b5e6fac041ce5326eeb8dc9ae4a2304112892d2
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
    "creator_id": 531,
    "id": 186,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "discipline_id": 193,
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
    "updated_at": "2016-12-08T18:10:03.648Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 193,
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
curl "api.goskive.com/v2/courses/186" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 816fa7b83a6c6d85286707ad0b5e6fac041ce5326eeb8dc9ae4a2304112892d2"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 28159597bcd17aaf5ee7fe5cc72179a1623844d1e094f2f295a2bc3aa056bdc9
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
    "creator_id": 536,
    "id": 189,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 168,
    "additional_university_ids": [

    ],
    "discipline_id": 196,
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
    "updated_at": "2016-12-08T18:10:04.126Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 196,
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
	-H "Authorization: Bearer 28159597bcd17aaf5ee7fe5cc72179a1623844d1e094f2f295a2bc3aa056bdc9"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 59131e20a9f5b2f0c14a02d86a906875ca7285ffec5936565703e03eb5858d0d
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
      "id": 6,
      "user_id": 87,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:20.201Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 91,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:20.502Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 95,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:20.793Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 99,
      "feedbackable_id": 7,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:21.090Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 103,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T18:09:21.382Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59131e20a9f5b2f0c14a02d86a906875ca7285ffec5936565703e03eb5858d0d"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 9013c67f59903b751778a10a779b6b1f8740164f541d7e646052f20276f53d8f
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
      "id": 15,
      "user_id": 124,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T18:09:22.911Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9013c67f59903b751778a10a779b6b1f8740164f541d7e646052f20276f53d8f"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer db6cc098675c4d86474e6d7658b72151902dcf8d05cfa1b1ca173b9a6ef9edc9
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
	-H "Authorization: Bearer db6cc098675c4d86474e6d7658b72151902dcf8d05cfa1b1ca173b9a6ef9edc9"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 8c6becd7d1d6f85b2f3ce3b65b644ff5c418ef847df27d9cb2830d73a1739a7a
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
      "id": 46,
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
      "created_at": "2016-12-08T18:09:17.706Z",
      "updated_at": "2016-12-08T18:09:17.706Z"
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
    "created_at": "2016-12-08T18:09:17.806Z",
    "updated_at": "2016-12-08T18:09:17.806Z",
    "course_id": 14,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c6becd7d1d6f85b2f3ce3b65b644ff5c418ef847df27d9cb2830d73a1739a7a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/80/feedbacks
Content-Type: application/json
Authorization: Bearer da8da08bd754dd09d30be61fce0f2de37f04697bedab2ce883c58e1fdaa1f4c7
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
      "user_id": 735,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:22.556Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 734,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:22.545Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/80/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da8da08bd754dd09d30be61fce0f2de37f04697bedab2ce883c58e1fdaa1f4c7"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 7f797256c66ea13b293c1ae62346354c117ffe4ef4a7ae091d7b86267d8966ee
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
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 702,
      "chapter_id": 130,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:20.158Z",
      "created_at": "2016-12-08T18:10:20.158Z",
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
      "author_id": 705,
      "chapter_id": 131,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:20.322Z",
      "created_at": "2016-12-08T18:10:20.322Z",
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
      "author_id": 708,
      "chapter_id": 132,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:20.487Z",
      "created_at": "2016-12-08T18:10:20.487Z",
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 711,
      "chapter_id": 133,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:20.654Z",
      "created_at": "2016-12-08T18:10:20.654Z",
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
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 714,
      "chapter_id": 134,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:20.821Z",
      "created_at": "2016-12-08T18:10:20.821Z",
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
	-H "Authorization: Bearer 7f797256c66ea13b293c1ae62346354c117ffe4ef4a7ae091d7b86267d8966ee"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 44412129d2ddf9a587ff1274ee59663730178538a8ea5fe58eb0863dcc258de9
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 682,
      "chapter_id": 124,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:19.040Z",
      "created_at": "2016-12-08T18:10:19.040Z",
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
	-H "Authorization: Bearer 44412129d2ddf9a587ff1274ee59663730178538a8ea5fe58eb0863dcc258de9"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/53/republish
Content-Type: application/json
Authorization: Bearer 1e0b11ebdd6706d22a68c53828294b82700a654f10a2bb4e7b6a3bddbe2aa736
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e0b11ebdd6706d22a68c53828294b82700a654f10a2bb4e7b6a3bddbe2aa736"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/66/feedbacks
Content-Type: application/json
Authorization: Bearer ea81d51cb19c51712825854e88c97823bd8f294842547cb6b573d959aa80a864
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
      "id": 34,
      "user_id": 513,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:01.498Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 512,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:01.486Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/66/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea81d51cb19c51712825854e88c97823bd8f294842547cb6b573d959aa80a864"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 4b23959ce2297dd5d0dd106012f9d427f8fd563122b38e0002af8fd84e61c80a
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
      "author_id": 336,
      "chapter_id": 66,
      "position": 45,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:47.895Z",
      "created_at": "2016-12-08T18:09:47.814Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 339,
      "chapter_id": 67,
      "position": 46,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:48.158Z",
      "created_at": "2016-12-08T18:09:48.076Z",
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
    },
    {
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 342,
      "chapter_id": 68,
      "position": 47,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:48.417Z",
      "created_at": "2016-12-08T18:09:48.334Z",
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
          "id": 107,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 108,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 345,
      "chapter_id": 69,
      "position": 48,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:48.688Z",
      "created_at": "2016-12-08T18:09:48.606Z",
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 348,
      "chapter_id": 70,
      "position": 49,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:48.946Z",
      "created_at": "2016-12-08T18:09:48.870Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b23959ce2297dd5d0dd106012f9d427f8fd563122b38e0002af8fd84e61c80a"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 80dc762b9bf602754aa98ee0563f5ba6ff88a92705c99f8d7b893b436b0b24a2
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
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 316,
      "chapter_id": 60,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:46.199Z",
      "created_at": "2016-12-08T18:09:46.127Z",
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
          "id": 91,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 92,
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
	-H "Authorization: Bearer 80dc762b9bf602754aa98ee0563f5ba6ff88a92705c99f8d7b893b436b0b24a2"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/57/republish
Content-Type: application/json
Authorization: Bearer e16a0449ca39eec0b68d5d9336bdcfa564c1d90bb2e5eedf6f97754ebaf3b46c
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
	-H "Authorization: Bearer e16a0449ca39eec0b68d5d9336bdcfa564c1d90bb2e5eedf6f97754ebaf3b46c"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fb692335c77a4c51aee38ff287541c3dc28b87b7d0341959693859afdab1124c
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":53,"published":false}}
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
    "creator_id": 185,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 48,
    "additional_university_ids": [

    ],
    "discipline_id": 53,
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
    "updated_at": "2016-12-08T18:09:27.868Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 53,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":53,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb692335c77a4c51aee38ff287541c3dc28b87b7d0341959693859afdab1124c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 33d75368112589106c02670867ada8c4d0fad00cedf1247a7f32d3e84a03fdf1
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
      "creator_id": 218,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-74",
      "html_url": "https://goskive.com/course/fu-course-74",
      "slug": "fu-course-74",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "discipline_id": 83,
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
      "updated_at": "2016-12-08T18:09:34.113Z",
      "shortname": "fu-course-74",
      "topic_id": 83,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 74",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 218,
      "id": 79,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-75",
      "html_url": "https://goskive.com/course/fu-course-75",
      "slug": "fu-course-75",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "discipline_id": 84,
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
      "updated_at": "2016-12-08T18:09:34.147Z",
      "shortname": "fu-course-75",
      "topic_id": 84,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 75",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 219,
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-76",
      "html_url": "https://goskive.com/course/fu-course-76",
      "slug": "fu-course-76",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "discipline_id": 85,
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
      "updated_at": "2016-12-08T18:09:34.189Z",
      "shortname": "fu-course-76",
      "topic_id": 85,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 76",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 219,
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-77",
      "html_url": "https://goskive.com/course/fu-course-77",
      "slug": "fu-course-77",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "discipline_id": 86,
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
      "chapters_updated_at": "2016-12-08T18:09:34.031Z",
      "updated_at": "2016-12-08T18:09:34.448Z",
      "shortname": "fu-course-77",
      "topic_id": 86,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 77",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33d75368112589106c02670867ada8c4d0fad00cedf1247a7f32d3e84a03fdf1"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2d758e39aae7e260d29d2b1a4a76d0684d69c6bc7583bee30a319c88cf8860da
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
      "creator_id": 224,
      "id": 82,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-78",
      "html_url": "https://goskive.com/course/fu-course-78",
      "slug": "fu-course-78",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "discipline_id": 87,
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
      "updated_at": "2016-12-08T18:09:34.673Z",
      "shortname": "fu-course-78",
      "topic_id": 87,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 78",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 224,
      "id": 83,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-79",
      "html_url": "https://goskive.com/course/fu-course-79",
      "slug": "fu-course-79",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "discipline_id": 88,
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
      "updated_at": "2016-12-08T18:09:34.708Z",
      "shortname": "fu-course-79",
      "topic_id": 88,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 79",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 225,
      "id": 84,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-80",
      "html_url": "https://goskive.com/course/fu-course-80",
      "slug": "fu-course-80",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "discipline_id": 89,
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
      "updated_at": "2016-12-08T18:09:34.750Z",
      "shortname": "fu-course-80",
      "topic_id": 89,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 80",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 225,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-81",
      "html_url": "https://goskive.com/course/fu-course-81",
      "slug": "fu-course-81",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "discipline_id": 90,
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
      "updated_at": "2016-12-08T18:09:34.783Z",
      "shortname": "fu-course-81",
      "topic_id": 90,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 81",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d758e39aae7e260d29d2b1a4a76d0684d69c6bc7583bee30a319c88cf8860da"
```
