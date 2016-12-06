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
DELETE /v2/bookmarks/3
Content-Type: application/json
Authorization: Bearer 53989515b2e3c78e40627906d09038a9ad8c0567b1f4103c063d4850b730be26
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53989515b2e3c78e40627906d09038a9ad8c0567b1f4103c063d4850b730be26"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 61c0d66648dd817e2a8a0089b1ee1883dad095ca39ddd952ec3b6d38f8b3eeb5
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":277,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":277,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61c0d66648dd817e2a8a0089b1ee1883dad095ca39ddd952ec3b6d38f8b3eeb5"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer da00d4d01e10c227ca2a7f8aef21c99e08f4c377f1e2a196c12711cd1fb5bc6c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":278,"pinned":true}}
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
    "course_id": 278,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-06T18:17:50.271Z",
    "course_published": true,
    "updated_at": "2016-12-06T18:17:50.263Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":278,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da00d4d01e10c227ca2a7f8aef21c99e08f4c377f1e2a196c12711cd1fb5bc6c"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/78/bookmarks
Content-Type: application/json
Authorization: Bearer 37febad3aff2cd7e13782591764d517825db900a44a03596b8258c500560f614
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
    "id": 7,
    "bookmarkable_id": 78,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/78/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37febad3aff2cd7e13782591764d517825db900a44a03596b8258c500560f614"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/57/votes
Content-Type: application/json
Authorization: Bearer 27aa314b81ed3cff073ad0addd60e5b6b0d4f590fc6a14b701516bb4c0a434fd
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
    "votable_id": 57,
    "user_id": 433
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27aa314b81ed3cff073ad0addd60e5b6b0d4f590fc6a14b701516bb4c0a434fd"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/109/bookmarks
Content-Type: application/json
Authorization: Bearer d9ff05ad7f903873b8975656005a623c2558786c42cb33de30575703f8db60f8
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
    "id": 9,
    "bookmarkable_id": 109,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/109/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9ff05ad7f903873b8975656005a623c2558786c42cb33de30575703f8db60f8"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/1/votes
Content-Type: application/json
Authorization: Bearer ef5c12f8966559a577856ae55fe02900ebe1cb0da9d806e248c39cb91469691d
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
    "votable_id": 1,
    "user_id": 1
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef5c12f8966559a577856ae55fe02900ebe1cb0da9d806e248c39cb91469691d"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/22
Content-Type: application/json
Authorization: Bearer 3d3d11c009a0d6fcda3c6c212a51dcb3078ad837b9480b048fe7b8be0d026f9b
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
    "id": 22,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 105,
    "user_id": 588
  }
}
```



```shell
curl "api.goskive.com/v2/votes/22" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d3d11c009a0d6fcda3c6c212a51dcb3078ad837b9480b048fe7b8be0d026f9b"
```
