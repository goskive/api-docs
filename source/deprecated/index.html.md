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
DELETE /v2/bookmarks/10
Content-Type: application/json
Authorization: Bearer bf542d3944c4c3f74ad66cfc27cafdf0af3348f45c8422e1bd996a92909087c0
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf542d3944c4c3f74ad66cfc27cafdf0af3348f45c8422e1bd996a92909087c0"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 650c518124a4d0034f640a80ddab4a4db2fae2a7303608015cf19afb7ea34261
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":254,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":254,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 650c518124a4d0034f640a80ddab4a4db2fae2a7303608015cf19afb7ea34261"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7c0f0f61386f9c95af8e89e52518a14dc31dbd42314fe5a08cc39a607cc5f8ae
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":253,"pinned":true}}
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
    "course_id": 253,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-24T09:02:36.619Z",
    "course_published": true,
    "updated_at": "2016-11-24T09:02:36.610Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":253,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c0f0f61386f9c95af8e89e52518a14dc31dbd42314fe5a08cc39a607cc5f8ae"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/82/bookmarks
Content-Type: application/json
Authorization: Bearer 523fee220098b51911ffcb54c62795bbbbb795c8a115f24f1d9eb4107a00b5a6
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
    "id": 9,
    "bookmarkable_id": 82,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 523fee220098b51911ffcb54c62795bbbbb795c8a115f24f1d9eb4107a00b5a6"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/3/votes
Content-Type: application/json
Authorization: Bearer 7b8c1dcd34eb7549375b3adf43c32a14be354ab3bdf370ad4bcd98a040f888fe
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 3,
    "user_id": 281
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b8c1dcd34eb7549375b3adf43c32a14be354ab3bdf370ad4bcd98a040f888fe"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/32/bookmarks
Content-Type: application/json
Authorization: Bearer b8f0724cbda321864b9c88de5320069b7f8493fbc660a127777b83ec08e66557
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
    "bookmarkable_id": 32,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/32/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8f0724cbda321864b9c88de5320069b7f8493fbc660a127777b83ec08e66557"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/94/votes
Content-Type: application/json
Authorization: Bearer a0a59d1e3e453ce316d5903702d88d20738c65543bcbf05b3462c6e29d4c2d29
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 94,
    "user_id": 650
  }
}
```



```shell
curl "api.goskive.com/v2/questions/94/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0a59d1e3e453ce316d5903702d88d20738c65543bcbf05b3462c6e29d4c2d29"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/20
Content-Type: application/json
Authorization: Bearer 2a5f3fd513993b692cb84dfe47ff406bc4127caee3f39c56a436a7fe5ac5d506
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
    "votable_id": 95,
    "user_id": 653
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a5f3fd513993b692cb84dfe47ff406bc4127caee3f39c56a436a7fe5ac5d506"
```
