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
DELETE /v2/bookmarks/2
Content-Type: application/json
Authorization: Bearer 8875e579ddeafda2110905a922012cfe27833e3e892ca8fb0aca8b1fe4e34ae8
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8875e579ddeafda2110905a922012cfe27833e3e892ca8fb0aca8b1fe4e34ae8"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3ce45928f2af486d623910ed1b2eb140158c36e4b5021176a671c8a786e6fa22
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":148,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":148,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ce45928f2af486d623910ed1b2eb140158c36e4b5021176a671c8a786e6fa22"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer e56116d21c02d50d257093ae331d04890c917712a7a7fe583177db513a3b98d1
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":149,"pinned":true}}
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
    "course_id": 149,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T10:04:16.459Z",
    "course_published": true,
    "updated_at": "2016-10-25T10:04:16.446Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":149,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e56116d21c02d50d257093ae331d04890c917712a7a7fe583177db513a3b98d1"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/46/bookmarks
Content-Type: application/json
Authorization: Bearer 221487da300a28397595bf5603ea190bc62377e61aaccfc653d1eacb09c147d6
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
    "id": 3,
    "bookmarkable_id": 46,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/46/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 221487da300a28397595bf5603ea190bc62377e61aaccfc653d1eacb09c147d6"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/7/votes
Content-Type: application/json
Authorization: Bearer 8917f9ccd53df9527b5a9baf0bd1d4200cc8e615000c0bb2c9e5a331cb599060
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 7,
    "user_id": 102
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/7/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8917f9ccd53df9527b5a9baf0bd1d4200cc8e615000c0bb2c9e5a331cb599060"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/81/bookmarks
Content-Type: application/json
Authorization: Bearer 81aa28d79bcbe52679a949ece8f096bb4e662e5d34b770589bc2f1e0d383d98d
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
    "id": 4,
    "bookmarkable_id": 81,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/81/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81aa28d79bcbe52679a949ece8f096bb4e662e5d34b770589bc2f1e0d383d98d"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/89/votes
Content-Type: application/json
Authorization: Bearer 5c603f47ca4f3c20e52ad569216e529834d343d84f1b7ada04200b49d648b2f6
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 89,
    "user_id": 544
  }
}
```



```shell
curl "api.goskive.com/v2/questions/89/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c603f47ca4f3c20e52ad569216e529834d343d84f1b7ada04200b49d648b2f6"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/6
Content-Type: application/json
Authorization: Bearer f6fb2866345fdf5cbe6db81678048e7455364470ff252534181b3737f5c6fac0
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 13,
    "user_id": 125
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6fb2866345fdf5cbe6db81678048e7455364470ff252534181b3737f5c6fac0"
```
