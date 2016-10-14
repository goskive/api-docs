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
Authorization: Bearer 0aea26ee707795e7261cfc4b9819d27150e1806437c8a669731e0b245e664eda
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
	-H "Authorization: Bearer 0aea26ee707795e7261cfc4b9819d27150e1806437c8a669731e0b245e664eda"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer eb358e82120c73da8b31fa914ea1544c823455f8219bce7908c965e6071c76d6
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":93,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":93,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb358e82120c73da8b31fa914ea1544c823455f8219bce7908c965e6071c76d6"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6f3342243169feef3fa395c1d5da64150cefb8552fe85302b44638d3994e4453
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":92,"pinned":true}}
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
    "id": 7,
    "course_id": 92,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T18:44:01.775Z",
    "course_published": true,
    "updated_at": "2016-10-14T18:44:01.766Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":92,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f3342243169feef3fa395c1d5da64150cefb8552fe85302b44638d3994e4453"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/44/bookmarks
Content-Type: application/json
Authorization: Bearer 5c31f3aa5abf48da7bfe60e0da09c499901562da9bc1e406a075e5e0d97cb1b5
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
    "bookmarkable_id": 44,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/44/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c31f3aa5abf48da7bfe60e0da09c499901562da9bc1e406a075e5e0d97cb1b5"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/91/votes
Content-Type: application/json
Authorization: Bearer 527c6fe1d38dbb75d789214a72c89c1c06f9b29fa27a524845680f279297f6df
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
    "votable_id": 91,
    "user_id": 748
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 527c6fe1d38dbb75d789214a72c89c1c06f9b29fa27a524845680f279297f6df"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/117/bookmarks
Content-Type: application/json
Authorization: Bearer c617d574b62f7b98a809e8479816f45f730223ea184fec32b0588740d55b943f
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
    "id": 5,
    "bookmarkable_id": 117,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/117/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c617d574b62f7b98a809e8479816f45f730223ea184fec32b0588740d55b943f"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer a6c19481e51761fd55e432874ba99cd56cef74488660f8d584af5608b5887a85
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
	-H "Authorization: Bearer a6c19481e51761fd55e432874ba99cd56cef74488660f8d584af5608b5887a85"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/12
Content-Type: application/json
Authorization: Bearer eb70e7eaf9a6bbb695d7d2b4f3c962b57d5c69d955ea75e629c9fa067b04f43a
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 81,
    "user_id": 395
  }
}
```



```shell
curl "api.goskive.com/v2/votes/12" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb70e7eaf9a6bbb695d7d2b4f3c962b57d5c69d955ea75e629c9fa067b04f43a"
```
