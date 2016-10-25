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
DELETE /v2/bookmarks/6
Content-Type: application/json
Authorization: Bearer 85d34c5e5beb4408c79efc231d53935cff53f100ed0cf21ad498458ca544980a
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85d34c5e5beb4408c79efc231d53935cff53f100ed0cf21ad498458ca544980a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 457f1b219cf613c85b4395e4a5b34859e7bbfbf5b3f9550f53d82bf0e2ef15c9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":96,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":96,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 457f1b219cf613c85b4395e4a5b34859e7bbfbf5b3f9550f53d82bf0e2ef15c9"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 01610c6380fb6a866a1ebbf5f2c55e2d4f8cbe75a72fa1225d08ea4bdc9bae59
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":95,"pinned":true}}
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
    "id": 5,
    "course_id": 95,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T09:28:22.304Z",
    "course_published": true,
    "updated_at": "2016-10-25T09:28:22.294Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":95,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01610c6380fb6a866a1ebbf5f2c55e2d4f8cbe75a72fa1225d08ea4bdc9bae59"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/18/bookmarks
Content-Type: application/json
Authorization: Bearer 97361df21d9d6fea3147f7dd284f42a041c931e1e970c9d2f6ba14b087f9464e
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
    "id": 1,
    "bookmarkable_id": 18,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/18/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97361df21d9d6fea3147f7dd284f42a041c931e1e970c9d2f6ba14b087f9464e"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/45/votes
Content-Type: application/json
Authorization: Bearer 5e8f2c8eb0c8076c5dcef6485530d6afa526c901c44fb8c822ff6b8c63fd8e24
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 45,
    "user_id": 241
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/45/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e8f2c8eb0c8076c5dcef6485530d6afa526c901c44fb8c822ff6b8c63fd8e24"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/89/bookmarks
Content-Type: application/json
Authorization: Bearer 325ce946b58243dacc2140951d3cd5479fc25ee1d5ffb8a6da61daf45034c111
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
    "id": 7,
    "bookmarkable_id": 89,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/89/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 325ce946b58243dacc2140951d3cd5479fc25ee1d5ffb8a6da61daf45034c111"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/28/votes
Content-Type: application/json
Authorization: Bearer 01d05a143c6308a501c0d5e34fbb391a758ffd4568d4e05fb7cac54d4b4a9f4f
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
    "votable_id": 28,
    "user_id": 165
  }
}
```



```shell
curl "api.goskive.com/v2/questions/28/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01d05a143c6308a501c0d5e34fbb391a758ffd4568d4e05fb7cac54d4b4a9f4f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/20
Content-Type: application/json
Authorization: Bearer 8893727ff5d9596f4221cdf43b1f9a86c00f868ae639611ba188e88b9e4288fa
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 132,
    "user_id": 958
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8893727ff5d9596f4221cdf43b1f9a86c00f868ae639611ba188e88b9e4288fa"
```
