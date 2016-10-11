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
DELETE /v2/bookmarks/4
Content-Type: application/json
Authorization: Bearer 0ff0d9cf8fd74d91ef1b1b45a28df611d79f13c8dfa98808205a629036782b58
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ff0d9cf8fd74d91ef1b1b45a28df611d79f13c8dfa98808205a629036782b58"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7c2bf8b4d5e4d33e53627a1e8bec48613aed825f4eabd5104080ba9cd5f3477b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":263,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":263,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c2bf8b4d5e4d33e53627a1e8bec48613aed825f4eabd5104080ba9cd5f3477b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f0d20b471cf88e8e3f576689e6abf0b2635adafb2c51eb2250c84e1ef33722d9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":264,"pinned":true}}
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
    "id": 8,
    "course_id": 264,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-11T17:00:25.211Z",
    "course_published": true,
    "updated_at": "2016-10-11T17:00:25.202Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":264,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0d20b471cf88e8e3f576689e6abf0b2635adafb2c51eb2250c84e1ef33722d9"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/84/bookmarks
Content-Type: application/json
Authorization: Bearer 02b8a4ff0bd6d2d787ecec699b71a83317906050aeb0837c0068dd7944033f67
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
    "bookmarkable_id": 84,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02b8a4ff0bd6d2d787ecec699b71a83317906050aeb0837c0068dd7944033f67"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/64/votes
Content-Type: application/json
Authorization: Bearer c0277a23470dac85c65d6426a58e9dbc50135353ba3d51712aaf1df47adfa538
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 64,
    "user_id": 430
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/64/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0277a23470dac85c65d6426a58e9dbc50135353ba3d51712aaf1df47adfa538"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/74/bookmarks
Content-Type: application/json
Authorization: Bearer f4a7c88268f1ec4aae76e05255040caa86fe2828ac682f02b22ce8d804914344
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
    "id": 3,
    "bookmarkable_id": 74,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/74/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4a7c88268f1ec4aae76e05255040caa86fe2828ac682f02b22ce8d804914344"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/27/votes
Content-Type: application/json
Authorization: Bearer b43c1ada6770bfbc87b693e176086a1aeb364d4f427376dc0a771b25748568e7
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 27,
    "user_id": 55
  }
}
```



```shell
curl "api.goskive.com/v2/questions/27/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b43c1ada6770bfbc87b693e176086a1aeb364d4f427376dc0a771b25748568e7"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/7
Content-Type: application/json
Authorization: Bearer 2186715153c38c34c71d4021e4256e2c4c07af67171f75a730dc0c4cf9da00a2
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 30,
    "user_id": 152
  }
}
```



```shell
curl "api.goskive.com/v2/votes/7" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2186715153c38c34c71d4021e4256e2c4c07af67171f75a730dc0c4cf9da00a2"
```
