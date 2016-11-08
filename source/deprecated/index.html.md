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
DELETE /v2/bookmarks/8
Content-Type: application/json
Authorization: Bearer 0d1846028ec42e91f378fc9aa6ce0b50177212ef8123e9dab6c112782dce207a
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d1846028ec42e91f378fc9aa6ce0b50177212ef8123e9dab6c112782dce207a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer d58dabb723bedd4d3b1b08c69e458e4d9cdc46024a2583b0e88926de78dc7b3b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":56,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":56,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d58dabb723bedd4d3b1b08c69e458e4d9cdc46024a2583b0e88926de78dc7b3b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 919649419253f819f19224cfc2255a33fa2ae5944bc4a94fe0bee4db7272ada3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":57,"pinned":true}}
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
    "id": 1,
    "course_id": 57,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T20:46:49.947Z",
    "course_published": true,
    "updated_at": "2016-11-08T20:46:49.937Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":57,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 919649419253f819f19224cfc2255a33fa2ae5944bc4a94fe0bee4db7272ada3"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/12/bookmarks
Content-Type: application/json
Authorization: Bearer b7048104463212fd072ae0189d52d67a4062ac77508e1d2d754220d78192bc2c
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
    "id": 2,
    "bookmarkable_id": 12,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/12/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7048104463212fd072ae0189d52d67a4062ac77508e1d2d754220d78192bc2c"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/93/votes
Content-Type: application/json
Authorization: Bearer f49b8a41c3807885cb17b48fdaa018f193163e7cc60dfb555249c7c147903517
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 93,
    "user_id": 807
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/93/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f49b8a41c3807885cb17b48fdaa018f193163e7cc60dfb555249c7c147903517"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/17/bookmarks
Content-Type: application/json
Authorization: Bearer 7d4e3529dd8613c376b979dfe64b87e367e6a43e76dc49d3de5f6565e31dc8fe
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
    "bookmarkable_id": 17,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/17/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d4e3529dd8613c376b979dfe64b87e367e6a43e76dc49d3de5f6565e31dc8fe"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/45/votes
Content-Type: application/json
Authorization: Bearer 3403ac43a2c9193d97a315c50ab92b356855d466a348443f60c844e4aa6d53c3
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 45,
    "user_id": 360
  }
}
```



```shell
curl "api.goskive.com/v2/questions/45/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3403ac43a2c9193d97a315c50ab92b356855d466a348443f60c844e4aa6d53c3"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/10
Content-Type: application/json
Authorization: Bearer 76327653fa2fdd431f8e2e828bc98f3cb9c29845af30b3099888a45b8c8ef1a7
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 47,
    "user_id": 369
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76327653fa2fdd431f8e2e828bc98f3cb9c29845af30b3099888a45b8c8ef1a7"
```
