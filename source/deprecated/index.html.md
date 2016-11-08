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
Authorization: Bearer ca00831beff8ffc34bbd3a0ab638cdcddb200e048ddd4c791a0ef5e45058b986
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
	-H "Authorization: Bearer ca00831beff8ffc34bbd3a0ab638cdcddb200e048ddd4c791a0ef5e45058b986"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8c7a41ca7d3393fcde294ba5f7714c01a1051a716dfe0a8dce5517ff6d5c5d31
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":6,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":6,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c7a41ca7d3393fcde294ba5f7714c01a1051a716dfe0a8dce5517ff6d5c5d31"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 17ca75bcb3d17317393c4a34f9c12c922d1fd4fff7229f107091c5729eb727cb
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":5,"pinned":true}}
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
    "course_id": 5,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T11:39:39.185Z",
    "course_published": true,
    "updated_at": "2016-11-08T11:39:39.176Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":5,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17ca75bcb3d17317393c4a34f9c12c922d1fd4fff7229f107091c5729eb727cb"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/58/bookmarks
Content-Type: application/json
Authorization: Bearer 6a2114b8a54e34d9ec8cbd005c293aed7a183bf3f918b4c38293e55d817db508
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
    "id": 10,
    "bookmarkable_id": 58,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/58/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a2114b8a54e34d9ec8cbd005c293aed7a183bf3f918b4c38293e55d817db508"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/55/votes
Content-Type: application/json
Authorization: Bearer 1eb1484622ec9a98567bd4edb0ef0041ffd20eff50c32713e90f7fcdaef106ad
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
    "votable_id": 55,
    "user_id": 757
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/55/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1eb1484622ec9a98567bd4edb0ef0041ffd20eff50c32713e90f7fcdaef106ad"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/70/bookmarks
Content-Type: application/json
Authorization: Bearer bc85a677f1217123df34167c6ba69f1cfcf4217b8f62746a7e865ee5a0346294
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
    "bookmarkable_id": 70,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/70/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc85a677f1217123df34167c6ba69f1cfcf4217b8f62746a7e865ee5a0346294"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/94/votes
Content-Type: application/json
Authorization: Bearer fcce7a1fbf67450d7642b05b108ec4286d51fd18ce8da1a7e17d89a372d514ee
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
    "votable_id": 94,
    "user_id": 810
  }
}
```



```shell
curl "api.goskive.com/v2/questions/94/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcce7a1fbf67450d7642b05b108ec4286d51fd18ce8da1a7e17d89a372d514ee"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/5
Content-Type: application/json
Authorization: Bearer 7a8ccb85da68b7fe569b4782672ee9762673bfd9760b740ac900936f754b5e7e
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 8,
    "user_id": 46
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a8ccb85da68b7fe569b4782672ee9762673bfd9760b740ac900936f754b5e7e"
```
