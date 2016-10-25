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
DELETE /v2/chapters/120
Content-Type: application/json
Authorization: Bearer 7953ae5bbe4b63ddcb610e3ed219416d7678198a9953956a87fc818d957058cb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/120" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7953ae5bbe4b63ddcb610e3ed219416d7678198a9953956a87fc818d957058cb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/114
Content-Type: application/json
Authorization: Bearer c3a136d096bce113bb2899cd8244017ef4cc8f537d458c1abaadc08444f74981
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
    "id": 114,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T09:28:38.878Z",
    "course_id": 148,
    "author_id": 549,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T09:28:38.331Z",
    "questions_updated_at": "2016-10-25T09:28:38.331Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 552,
        "chapter_id": 114,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.826Z",
        "created_at": "2016-10-25T09:28:38.826Z",
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
        "author_id": 553,
        "chapter_id": 114,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.862Z",
        "created_at": "2016-10-25T09:28:38.862Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 550,
        "chapter_id": 114,
        "position": 77,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.574Z",
        "created_at": "2016-10-25T09:28:38.469Z",
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
            "id": 164,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 165,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 551,
        "chapter_id": 114,
        "position": 78,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.760Z",
        "created_at": "2016-10-25T09:28:38.644Z",
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
            "id": 166,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 167,
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
curl "api.goskive.com/v2/chapters/114" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3a136d096bce113bb2899cd8244017ef4cc8f537d458c1abaadc08444f74981"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/115
Content-Type: application/json
Authorization: Bearer f12e9290ae6665a4db337414456a5192a5fc63d72a8c1494c7f82101443823f5
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
    "id": 115,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T09:28:39.081Z",
    "course_id": 149,
    "author_id": 556,
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
curl "api.goskive.com/v2/chapters/115" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f12e9290ae6665a4db337414456a5192a5fc63d72a8c1494c7f82101443823f5"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer 378c6d3bde1cec7f0cc299a14cc382931a0ec448f0f2fc583c8342fd71a73b02
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
	-H "Authorization: Bearer 378c6d3bde1cec7f0cc299a14cc382931a0ec448f0f2fc583c8342fd71a73b02"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer cada5098d04a09b7d78657faf2b4a5e271e5e833971ba721024896a9adf2ebfa
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
      "id": 23,
      "author_id": 648,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:46.790Z",
      "status": "published",
      "subject_id": 204,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 650,
      "reply_to_id": 23,
      "created_at": "2016-10-25T09:28:46.871Z",
      "status": "published",
      "subject_id": 205,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 652,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:46.954Z",
      "status": "published",
      "subject_id": 206,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 654,
      "reply_to_id": 25,
      "created_at": "2016-10-25T09:28:47.037Z",
      "status": "published",
      "subject_id": 207,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 656,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:47.148Z",
      "status": "reported",
      "subject_id": 208,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 658,
      "reply_to_id": 27,
      "created_at": "2016-10-25T09:28:47.229Z",
      "status": "published",
      "subject_id": 209,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 660,
      "reply_to_id": 27,
      "created_at": "2016-10-25T09:28:47.310Z",
      "status": "published",
      "subject_id": 210,
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
	-H "Authorization: Bearer cada5098d04a09b7d78657faf2b4a5e271e5e833971ba721024896a9adf2ebfa"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 84f20062d7b12e35fce5bfffb34bc4b2692ef36509d0c2e0b78c791f3b2c3073
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
      "id": 30,
      "author_id": 663,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:47.446Z",
      "status": "published",
      "subject_id": 211,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 665,
      "reply_to_id": 30,
      "created_at": "2016-10-25T09:28:47.529Z",
      "status": "published",
      "subject_id": 212,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 667,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:47.609Z",
      "status": "published",
      "subject_id": 213,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 669,
      "reply_to_id": 32,
      "created_at": "2016-10-25T09:28:47.688Z",
      "status": "published",
      "subject_id": 214,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 671,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:47.769Z",
      "status": "reported",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 673,
      "reply_to_id": 34,
      "created_at": "2016-10-25T09:28:47.854Z",
      "status": "published",
      "subject_id": 216,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 675,
      "reply_to_id": 34,
      "created_at": "2016-10-25T09:28:47.936Z",
      "status": "published",
      "subject_id": 217,
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
	-H "Authorization: Bearer 84f20062d7b12e35fce5bfffb34bc4b2692ef36509d0c2e0b78c791f3b2c3073"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 542cc1d34277e89190d9f659f5613987cd63eb272d0055e1a6942fc97d940c63
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
      "id": 38,
      "author_id": 680,
      "reply_to_id": 37,
      "created_at": "2016-10-25T09:28:48.154Z",
      "status": "published",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 684,
      "reply_to_id": 39,
      "created_at": "2016-10-25T09:28:48.315Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 688,
      "reply_to_id": 41,
      "created_at": "2016-10-25T09:28:48.475Z",
      "status": "published",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 690,
      "reply_to_id": 41,
      "created_at": "2016-10-25T09:28:48.557Z",
      "status": "published",
      "subject_id": 224,
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
	-H "Authorization: Bearer 542cc1d34277e89190d9f659f5613987cd63eb272d0055e1a6942fc97d940c63"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer dd6516a28a18fb6f29e715f4fa4eab83d7ffb054fb7c0e6b99bbe2d23d845887
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
      "id": 20,
      "author_id": 641,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:46.504Z",
      "status": "reported",
      "subject_id": 201,
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
	-H "Authorization: Bearer dd6516a28a18fb6f29e715f4fa4eab83d7ffb054fb7c0e6b99bbe2d23d845887"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/55/republish
Content-Type: application/json
Authorization: Bearer cb61f79077e1e2754bcb45cf8c842ba1aff1f3a67429dbc5e286c97168d9645b
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb61f79077e1e2754bcb45cf8c842ba1aff1f3a67429dbc5e286c97168d9645b"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c0a0fbf827fec159ef36556c4ac8a161b958a0f985c06808656e10755cb4ba3e
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
    "id": 190,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T09:29:07.635Z",
    "course_id": 303,
    "author_id": 951,
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
	-H "Authorization: Bearer c0a0fbf827fec159ef36556c4ac8a161b958a0f985c06808656e10755cb4ba3e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/306/chapters
Content-Type: application/json
Authorization: Bearer fd2809f6cf19b9b48ec73239144beb641f47331c7664462ba95958e897474dc6
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
    "id": 192,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T09:29:07.986Z",
    "course_id": 306,
    "author_id": 957,
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
curl "api.goskive.com/v2/courses/306/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd2809f6cf19b9b48ec73239144beb641f47331c7664462ba95958e897474dc6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f0fc844390c6dacab1dffa31e2b65f291a581902db6e5c3e7899f5bcba6531bf
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
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-25T09:29:05.894Z",
      "course_id": 295,
      "author_id": 916,
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
      "id": 176,
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-25T09:29:05.917Z",
      "course_id": 295,
      "author_id": 917,
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
      "id": 177,
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-25T09:29:06.162Z",
      "course_id": 295,
      "author_id": 918,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T09:29:05.821Z",
      "questions_updated_at": "2016-10-25T09:29:05.821Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0fc844390c6dacab1dffa31e2b65f291a581902db6e5c3e7899f5bcba6531bf"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 15feee39c065e9527024cb919766697dab64434d2f9e150ef3e10f97a83b9ffa
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
      "title": "Clever Chapter Title 157",
      "position": 1,
      "updated_at": "2016-10-25T09:29:06.303Z",
      "course_id": 296,
      "author_id": 923,
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
      "id": 179,
      "title": "Clever Chapter Title 158",
      "position": 2,
      "updated_at": "2016-10-25T09:29:06.326Z",
      "course_id": 296,
      "author_id": 924,
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
      "id": 180,
      "title": "Clever Chapter Title 159",
      "position": 3,
      "updated_at": "2016-10-25T09:29:06.349Z",
      "course_id": 296,
      "author_id": 925,
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
	-H "Authorization: Bearer 15feee39c065e9527024cb919766697dab64434d2f9e150ef3e10f97a83b9ffa"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e34c4ac238f50fd6cdf527d6285b9f9085be0c49a6cb69ca1974661d7fb12aec
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
	-H "Authorization: Bearer e34c4ac238f50fd6cdf527d6285b9f9085be0c49a6cb69ca1974661d7fb12aec"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/61
Content-Type: application/json
Authorization: Bearer 972fe0e4d9dfd5b12818aa3902dd682736f11208bf6c4a852df54539b26799e0
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/61" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 972fe0e4d9dfd5b12818aa3902dd682736f11208bf6c4a852df54539b26799e0"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 7552a5028fc6730c2f613a9b44efcc2e6305c0b013d8dffcecada4565fd6f9b4
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
    "creator_id": 204,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 51,
    "additional_university_ids": [

    ],
    "topic_id": 52,
    "discipline_id": 52,
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
    "chapters_updated_at": "2016-10-25T09:28:07.030Z",
    "updated_at": "2016-10-25T09:28:08.653Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 42,
        "title": "Clever Chapter Title 39",
        "position": 1,
        "updated_at": "2016-10-25T09:28:08.605Z",
        "course_id": 50,
        "author_id": 204,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T09:28:07.030Z",
        "questions_updated_at": "2016-10-25T09:28:07.030Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 43,
        "title": "Clever Chapter Title 40",
        "position": 2,
        "updated_at": "2016-10-25T09:28:08.645Z",
        "course_id": 50,
        "author_id": 204,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T09:28:07.030Z",
        "questions_updated_at": "2016-10-25T09:28:07.030Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 204,
        "chapter_id": 42,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.433Z",
        "created_at": "2016-10-25T09:28:08.433Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 204,
        "chapter_id": 43,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.510Z",
        "created_at": "2016-10-25T09:28:08.510Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 204,
        "chapter_id": 42,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.477Z",
        "created_at": "2016-10-25T09:28:08.477Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 204,
        "chapter_id": 43,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.554Z",
        "created_at": "2016-10-25T09:28:08.554Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 207,
        "chapter_id": 42,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.594Z",
        "created_at": "2016-10-25T09:28:08.594Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 208,
        "chapter_id": 43,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.634Z",
        "created_at": "2016-10-25T09:28:08.634Z",
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
	-H "Authorization: Bearer 7552a5028fc6730c2f613a9b44efcc2e6305c0b013d8dffcecada4565fd6f9b4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/44
Content-Type: application/json
Authorization: Bearer 11e3469b317b2acf33b587e86635790bdd6ce484680f7bcbfb6949dec8fa3a68
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
    "creator_id": 189,
    "id": 44,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 45,
    "additional_university_ids": [

    ],
    "topic_id": 46,
    "discipline_id": 46,
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
    "updated_at": "2016-10-25T09:28:04.842Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/44" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11e3469b317b2acf33b587e86635790bdd6ce484680f7bcbfb6949dec8fa3a68"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6b079b4d1c4ed558754dab6f7005ec34cc130d8c4da226429a8741278bce6049
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
    "creator_id": 194,
    "id": 47,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 48,
    "additional_university_ids": [

    ],
    "topic_id": 49,
    "discipline_id": 49,
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
    "updated_at": "2016-10-25T09:28:05.211Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b079b4d1c4ed558754dab6f7005ec34cc130d8c4da226429a8741278bce6049"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer b787db750bc11f41be97058dea8c79f8dfa4fd8aed6b5674d59093ace41bb957
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
      "user_id": 68,
      "feedbackable_id": 9,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:27:55.814Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 72,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:27:56.097Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 76,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:27:56.385Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 80,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:27:56.680Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 84,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T09:27:56.976Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b787db750bc11f41be97058dea8c79f8dfa4fd8aed6b5674d59093ace41bb957"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 89ff7bf871582ab1f240c67e564d08c4c47c08055dd729958d9db967647941b8
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
      "user_id": 105,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T09:27:58.487Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89ff7bf871582ab1f240c67e564d08c4c47c08055dd729958d9db967647941b8"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer feb4211fb221532672836a634539b16b13a8ab49a0975602e54ff04c9ba03d3b
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
	-H "Authorization: Bearer feb4211fb221532672836a634539b16b13a8ab49a0975602e54ff04c9ba03d3b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/6/metadata
Content-Type: application/json
Authorization: Bearer 0427785807bbf8e8707e5b36fb5886a5bd8d6a699be33416e710233880728033
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
    "id": 6,
    "uploader": {
      "id": 331,
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
      "created_at": "2016-10-25T09:28:20.835Z",
      "updated_at": "2016-10-25T09:28:20.835Z"
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
    "created_at": "2016-10-25T09:28:20.907Z",
    "updated_at": "2016-10-25T09:28:20.907Z",
    "course_id": 86,
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
curl "api.goskive.com/v2/files/6/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0427785807bbf8e8707e5b36fb5886a5bd8d6a699be33416e710233880728033"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/50/feedbacks
Content-Type: application/json
Authorization: Bearer 27affd0a5e13a1e171be54adec5b1291a8640fbb9cae1adb67570cecd3e923e7
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
      "id": 32,
      "user_id": 271,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:15.814Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 270,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:15.804Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27affd0a5e13a1e171be54adec5b1291a8640fbb9cae1adb67570cecd3e923e7"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer f172b2e0dd957e76e60c7426813a174344629efebc886f054973655f9d953127
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 415,
      "chapter_id": 81,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:27.723Z",
      "created_at": "2016-10-25T09:28:27.723Z",
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 418,
      "chapter_id": 82,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:27.863Z",
      "created_at": "2016-10-25T09:28:27.863Z",
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 421,
      "chapter_id": 83,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:28.003Z",
      "created_at": "2016-10-25T09:28:28.003Z",
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 424,
      "chapter_id": 84,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:28.143Z",
      "created_at": "2016-10-25T09:28:28.143Z",
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 427,
      "chapter_id": 85,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:28.282Z",
      "created_at": "2016-10-25T09:28:28.282Z",
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
	-H "Authorization: Bearer f172b2e0dd957e76e60c7426813a174344629efebc886f054973655f9d953127"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 6f5686a259a406a234dc18222a2e874506e5285aafb51f0c337dc09d156f1fbb
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 443,
      "chapter_id": 90,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:29.030Z",
      "created_at": "2016-10-25T09:28:29.030Z",
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
	-H "Authorization: Bearer 6f5686a259a406a234dc18222a2e874506e5285aafb51f0c337dc09d156f1fbb"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/81/republish
Content-Type: application/json
Authorization: Bearer c2834e1b8bd39f1514bf8929226f36fe92954269b12386cb044901d6c7560f1e
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/81/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2834e1b8bd39f1514bf8929226f36fe92954269b12386cb044901d6c7560f1e"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/97/feedbacks
Content-Type: application/json
Authorization: Bearer 11a7b7bffa09182ce92937f7882d5626bf7f416b732bc6002d120ffedb1aae34
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
      "id": 40,
      "user_id": 795,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:54.722Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 794,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:54.710Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/97/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11a7b7bffa09182ce92937f7882d5626bf7f416b732bc6002d120ffedb1aae34"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 7dd84839ffb8f4d557f14f3877a8901878b0ef66496a98b4ec67470f7b2d7216
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
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 851,
      "chapter_id": 152,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:00.275Z",
      "created_at": "2016-10-25T09:29:00.160Z",
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
          "id": 227,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 228,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 854,
      "chapter_id": 153,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:00.545Z",
      "created_at": "2016-10-25T09:29:00.430Z",
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
          "id": 229,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 230,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 857,
      "chapter_id": 154,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:00.819Z",
      "created_at": "2016-10-25T09:29:00.702Z",
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
          "id": 231,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 232,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 860,
      "chapter_id": 155,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:01.095Z",
      "created_at": "2016-10-25T09:29:00.976Z",
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
      "author_id": 863,
      "chapter_id": 156,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:01.365Z",
      "created_at": "2016-10-25T09:29:01.252Z",
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
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dd84839ffb8f4d557f14f3877a8901878b0ef66496a98b4ec67470f7b2d7216"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 742efa1a9d0d835f42978855c8ac349ad6075b55936f96722c444e078ae6d2f0
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
      "id": 126,
      "obfuscated_id": "fKTMLttUR-w",
      "author_id": 895,
      "chapter_id": 166,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:29:04.259Z",
      "created_at": "2016-10-25T09:29:04.145Z",
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
          "id": 255,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 256,
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
	-H "Authorization: Bearer 742efa1a9d0d835f42978855c8ac349ad6075b55936f96722c444e078ae6d2f0"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/105/republish
Content-Type: application/json
Authorization: Bearer 482be60b020ecb811245052d5d9d6d529a429f76ab122a30b7dad74857d5a075
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/105/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 482be60b020ecb811245052d5d9d6d529a429f76ab122a30b7dad74857d5a075"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 29e330892b4b75e5a45ea27d6b6642ee6447c38ac8e50d7ce289e9331adc1217
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":168,"published":false}}
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
    "creator_id": 575,
    "id": 156,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "topic_id": 168,
    "discipline_id": 169,
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
    "updated_at": "2016-10-25T09:28:40.333Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":168,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29e330892b4b75e5a45ea27d6b6642ee6447c38ac8e50d7ce289e9331adc1217"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6155f66024a8ce372fcff564997cc8d0d895174f23b81246c9b929865e835740
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
      "creator_id": 583,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-113",
      "html_url": "https://goskive.com/course/fu-course-113",
      "slug": "fu-course-113",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 113",
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
      "updated_at": "2016-10-25T09:28:41.131Z",
      "shortname": "fu-course-113"
    },
    {
      "creator_id": 583,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-114",
      "html_url": "https://goskive.com/course/fu-course-114",
      "slug": "fu-course-114",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 114",
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
      "updated_at": "2016-10-25T09:28:41.169Z",
      "shortname": "fu-course-114"
    },
    {
      "creator_id": 584,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 179,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T09:28:41.239Z",
      "shortname": "fu-course-115"
    },
    {
      "creator_id": 584,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-116",
      "html_url": "https://goskive.com/course/fu-course-116",
      "slug": "fu-course-116",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 180,
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
      "chapters_updated_at": "2016-10-25T09:28:41.515Z",
      "updated_at": "2016-10-25T09:28:41.521Z",
      "shortname": "fu-course-116"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6155f66024a8ce372fcff564997cc8d0d895174f23b81246c9b929865e835740"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c15181f364338e6990a1c620d6d03db539f8c720f940bf9e36be314d9671d5e4
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
      "creator_id": 589,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-117",
      "html_url": "https://goskive.com/course/fu-course-117",
      "slug": "fu-course-117",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 181,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T09:28:41.662Z",
      "shortname": "fu-course-117"
    },
    {
      "creator_id": 589,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-118",
      "html_url": "https://goskive.com/course/fu-course-118",
      "slug": "fu-course-118",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 182,
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
      "updated_at": "2016-10-25T09:28:41.700Z",
      "shortname": "fu-course-118"
    },
    {
      "creator_id": 590,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 183,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T09:28:41.745Z",
      "shortname": "fu-course-119"
    },
    {
      "creator_id": 590,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 183,
      "discipline_id": 184,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-25T09:28:41.783Z",
      "shortname": "fu-course-120"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c15181f364338e6990a1c620d6d03db539f8c720f940bf9e36be314d9671d5e4"
```
