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
Authorization: Bearer 47ced7da69a93813ffb2999dcf4a775cb4c6f60168a0ddd9d53c57c59ddf9993
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
	-H "Authorization: Bearer 47ced7da69a93813ffb2999dcf4a775cb4c6f60168a0ddd9d53c57c59ddf9993"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 75d80554e9c2993897e7382a51848d20f6fb9eb0b762e6e048c8c96e2737ea3d
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":280,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":280,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75d80554e9c2993897e7382a51848d20f6fb9eb0b762e6e048c8c96e2737ea3d"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 13aa2c60a6d124d5be363967672629698f81d233143e09b71bb746f3e8eb1d00
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":279,"pinned":true}}
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
    "course_id": 279,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T12:11:41.876Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:11:41.867Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":279,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13aa2c60a6d124d5be363967672629698f81d233143e09b71bb746f3e8eb1d00"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/68/bookmarks
Content-Type: application/json
Authorization: Bearer b720f2f69d31232922ed45e5204d30d847edba07da7a01fe985c89edc9083126
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
    "id": 6,
    "bookmarkable_id": 68,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/68/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b720f2f69d31232922ed45e5204d30d847edba07da7a01fe985c89edc9083126"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/58/votes
Content-Type: application/json
Authorization: Bearer 25a7635c24daa4a2cb47d3d52f906332e807d2e2f83e26bec6a09469a15cbb33
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 58,
    "user_id": 409
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/58/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25a7635c24daa4a2cb47d3d52f906332e807d2e2f83e26bec6a09469a15cbb33"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/1/bookmarks
Content-Type: application/json
Authorization: Bearer f19495c81435786dcf4f30ec211661c6102de0e486d5817547e0c4dd29f775fe
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
    "bookmarkable_id": 1,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f19495c81435786dcf4f30ec211661c6102de0e486d5817547e0c4dd29f775fe"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/107/votes
Content-Type: application/json
Authorization: Bearer 736bfc6866b4e00270262b83c1e712064a9867fdf8db0c1ed867bc105d6ef918
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 107,
    "user_id": 860
  }
}
```



```shell
curl "api.goskive.com/v2/questions/107/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 736bfc6866b4e00270262b83c1e712064a9867fdf8db0c1ed867bc105d6ef918"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer afd28dafc5c646165fcef7ab1499c8e5d0209507517d7ee8793a8a43bd05f608
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 104,
    "user_id": 769
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afd28dafc5c646165fcef7ab1499c8e5d0209507517d7ee8793a8a43bd05f608"
```
