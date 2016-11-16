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
DELETE /v2/bookmarks/5
Content-Type: application/json
Authorization: Bearer b5261507b77b15b014413c6255770161c28e585be2b1d5ef1b6197911fd82d49
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5261507b77b15b014413c6255770161c28e585be2b1d5ef1b6197911fd82d49"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8874ed5e2d12636c08edddacba1095eedbacb836641382fa9fdec11086102728
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":234,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":234,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8874ed5e2d12636c08edddacba1095eedbacb836641382fa9fdec11086102728"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1b020241f4e8a8942a9749116c52d1375bcd74f05a3465bcc76ca973491f2db9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":233,"pinned":true}}
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
    "course_id": 233,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-16T17:23:52.422Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:23:52.413Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":233,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b020241f4e8a8942a9749116c52d1375bcd74f05a3465bcc76ca973491f2db9"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/71/bookmarks
Content-Type: application/json
Authorization: Bearer 8fdcc71a04f22762ee352f876311b61f3603b56f9bdca17063f912c9305f2146
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
    "bookmarkable_id": 71,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/71/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fdcc71a04f22762ee352f876311b61f3603b56f9bdca17063f912c9305f2146"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/25/votes
Content-Type: application/json
Authorization: Bearer 5728e79016b2d9770ef6b6cf3a9aa58e9785f3bd827416d342de5a1a0833cf6d
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 25,
    "user_id": 433
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/25/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5728e79016b2d9770ef6b6cf3a9aa58e9785f3bd827416d342de5a1a0833cf6d"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/25/bookmarks
Content-Type: application/json
Authorization: Bearer 1db4f149efe5149ca191c47717bcd25096af056ffd735354d53f04d1fcaff4a9
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
    "id": 2,
    "bookmarkable_id": 25,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/25/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1db4f149efe5149ca191c47717bcd25096af056ffd735354d53f04d1fcaff4a9"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/30/votes
Content-Type: application/json
Authorization: Bearer 8e841c65e504e0d6c390a9735666f7573a3ef84e3de66b47220f676a50c309de
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
    "votable_id": 30,
    "user_id": 346
  }
}
```



```shell
curl "api.goskive.com/v2/questions/30/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e841c65e504e0d6c390a9735666f7573a3ef84e3de66b47220f676a50c309de"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/21
Content-Type: application/json
Authorization: Bearer f1695915cc1ce9f9fc179edae50b0188ec50649ffc44401051ad031d673914df
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
    "id": 21,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 131,
    "user_id": 885
  }
}
```



```shell
curl "api.goskive.com/v2/votes/21" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1695915cc1ce9f9fc179edae50b0188ec50649ffc44401051ad031d673914df"
```
