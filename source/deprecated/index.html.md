---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# Bookmarks

## Delete a bookmark

DEPRECATED. Use DELETE /v2/:content_unit_type/:content_unit_id/bookmark instead.

### Request

#### Endpoint

```
DELETE /v2/bookmarks/7
Content-Type: application/json
Authorization: Bearer 5cf8d3192bdd136224344574e2783de17f27199afb3c77f2506aed3f7a268cf2
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5cf8d3192bdd136224344574e2783de17f27199afb3c77f2506aed3f7a268cf2"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0f7f16360ca23069d801249214f1b5ab86d51eaace39f9ee06bd194f9bbc39a0
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":228,"pinned":true}}
```


| Name | Description |
|:-----|:------------|
| user_course[course_id] *required* | Course ID |
| user_course[pinned]  | Pinned |



### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":228,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f7f16360ca23069d801249214f1b5ab86d51eaace39f9ee06bd194f9bbc39a0"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 53b4515adcfc3d920391bee00bf24054d550a6b0825027b092b619b6c8ea0029
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":227,"pinned":true}}
```


| Name | Description |
|:-----|:------------|
| user_course[course_id] *required* | Course ID |
| user_course[pinned]  | Pinned |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "user_course": {
    "id": 4,
    "course_id": 227,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T12:25:44.332Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:25:44.322Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":227,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53b4515adcfc3d920391bee00bf24054d550a6b0825027b092b619b6c8ea0029"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer fbc18f1c0c5b2824cff9203da2cc717db3a98e073180f22f3ad94fda965b66af
```

`POST /v2/flashcards/:flashcard_id/bookmarks`

#### Parameters


```json
{}
```

None known.


### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "bookmark": {
    "id": 8,
    "bookmarkable_id": 95,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbc18f1c0c5b2824cff9203da2cc717db3a98e073180f22f3ad94fda965b66af"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/84/votes
Content-Type: application/json
Authorization: Bearer f1cdfe6dc09f65c66b80cffcc2d69bd7b0c66f604f8ab90098c5b951bfb7e25b
```

`POST /v2/flashcards/:flashcard_id/votes`

#### Parameters


```json
{"vote":{"type":"DownVote"}}
```


| Name | Description |
|:-----|:------------|
| vote[type] *required* | Vote type |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "vote": {
    "id": 19,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 84,
    "user_id": 895
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1cdfe6dc09f65c66b80cffcc2d69bd7b0c66f604f8ab90098c5b951bfb7e25b"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/21/bookmarks
Content-Type: application/json
Authorization: Bearer 3c1c0f188851bdcec747f82b9379e27dbd8743637f68d8f27cd4c4c639487e6f
```

`POST /v2/questions/:question_id/bookmarks`

#### Parameters


```json
{}
```

None known.


### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "bookmark": {
    "id": 1,
    "bookmarkable_id": 21,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/21/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c1c0f188851bdcec747f82b9379e27dbd8743637f68d8f27cd4c4c639487e6f"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer 5e32d753cf7b8657de36db728a7d5db21fafaa274d332168b301e52f45f10179
```

`POST /v2/questions/:question_id/votes`

#### Parameters


```json
{"vote":{"type":"DownVote"}}
```


| Name | Description |
|:-----|:------------|
| vote[type] *required* | Vote type |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "vote": {
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 10
  }
}
```



```shell
curl "api.goskive.com/v2/questions/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e32d753cf7b8657de36db728a7d5db21fafaa274d332168b301e52f45f10179"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/13
Content-Type: application/json
Authorization: Bearer e5b740120e7ee2739e69f123e82510ef292d412abe6b5193aa74fa71b368e090
```

`PATCH /v2/votes/:vote_id`

#### Parameters


```json
{"vote":{"type":"DownVote"}}
```


| Name | Description |
|:-----|:------------|
| vote[type] *required* | Vote type |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "vote": {
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 85,
    "user_id": 587
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5b740120e7ee2739e69f123e82510ef292d412abe6b5193aa74fa71b368e090"
```
