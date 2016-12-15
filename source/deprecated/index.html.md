---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Bookmarks

## Delete a bookmark

DEPRECATED. Use DELETE /v2/:content_unit_type/:content_unit_id/bookmark instead.

### Request

#### Endpoint

```
DELETE /v2/bookmarks/9
Content-Type: application/json
Authorization: Bearer 13a6f4ed0b0dcfb1f488542c1ad2eb4b99af76507a5b3f9ae5fc33cf6b80b2ab
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13a6f4ed0b0dcfb1f488542c1ad2eb4b99af76507a5b3f9ae5fc33cf6b80b2ab"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 73dee93886ef999b26d4ef4d09412b508364c0a220a8a1d09feed25f21926999
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":203,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":203,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73dee93886ef999b26d4ef4d09412b508364c0a220a8a1d09feed25f21926999"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7c160b55b134e99bc19d193c7a5192647944d03e87b5c858ace0361aecf8cbbe
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":202,"pinned":true}}
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
    "course_id": 202,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T11:57:19.274Z",
    "course_published": true,
    "updated_at": "2016-12-15T11:57:19.269Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":202,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c160b55b134e99bc19d193c7a5192647944d03e87b5c858ace0361aecf8cbbe"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/29/bookmarks
Content-Type: application/json
Authorization: Bearer 0c1009c96242440ae02f8ed182f9206b010bef1d14edcc6a7b58cc8092b36f9c
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
    "bookmarkable_id": 29,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c1009c96242440ae02f8ed182f9206b010bef1d14edcc6a7b58cc8092b36f9c"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/43/votes
Content-Type: application/json
Authorization: Bearer 74d0e2420ba521bfed7142754c7414a290c62a866ae5834db286ba3ae1076072
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 43,
    "user_id": 382
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74d0e2420ba521bfed7142754c7414a290c62a866ae5834db286ba3ae1076072"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/129/bookmarks
Content-Type: application/json
Authorization: Bearer e8c48d27559a12b23d6f3779eb2e9f50da62b47e8184e4c479a736d57d0d4f61
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
    "id": 8,
    "bookmarkable_id": 129,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/129/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8c48d27559a12b23d6f3779eb2e9f50da62b47e8184e4c479a736d57d0d4f61"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/48/votes
Content-Type: application/json
Authorization: Bearer 2b90309586a8e9f6b7ed366c3e10179d6a02006c9c3d84b80f4753978c9d8a1e
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 48,
    "user_id": 479
  }
}
```



```shell
curl "api.goskive.com/v2/questions/48/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b90309586a8e9f6b7ed366c3e10179d6a02006c9c3d84b80f4753978c9d8a1e"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/8
Content-Type: application/json
Authorization: Bearer 68e3e23879a5a32791358def30c29e20dd71f6a0df0688af4768e80f6e92e74e
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 17,
    "user_id": 181
  }
}
```



```shell
curl "api.goskive.com/v2/votes/8" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68e3e23879a5a32791358def30c29e20dd71f6a0df0688af4768e80f6e92e74e"
```
