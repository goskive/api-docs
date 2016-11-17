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
Authorization: Bearer 02dc95662cac448e0abd534b63ee60843dc10adb505f37e34ea306d3dc37d4a2
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
	-H "Authorization: Bearer 02dc95662cac448e0abd534b63ee60843dc10adb505f37e34ea306d3dc37d4a2"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 27798eb1bb8df7550e3a24b1e1a640588aaf51306b7e159bd32e46184903e591
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":29,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":29,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27798eb1bb8df7550e3a24b1e1a640588aaf51306b7e159bd32e46184903e591"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2de65f29b8fc3626133c52cceb9ae7ba379a65046136142e0eeace9e1b7a704b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":30,"pinned":true}}
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
    "course_id": 30,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-17T18:15:57.782Z",
    "course_published": true,
    "updated_at": "2016-11-17T18:15:57.773Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":30,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2de65f29b8fc3626133c52cceb9ae7ba379a65046136142e0eeace9e1b7a704b"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/87/bookmarks
Content-Type: application/json
Authorization: Bearer fc1ca502da86eb5fe6a9654a699a4a1c9e51e8dd665ad2813befabd70223e729
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
    "bookmarkable_id": 87,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc1ca502da86eb5fe6a9654a699a4a1c9e51e8dd665ad2813befabd70223e729"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/82/votes
Content-Type: application/json
Authorization: Bearer 9209cda4c9b2fda64548c3b1b62496e46b0266da49f8a7614fd266911252d960
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 82,
    "user_id": 818
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9209cda4c9b2fda64548c3b1b62496e46b0266da49f8a7614fd266911252d960"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/67/bookmarks
Content-Type: application/json
Authorization: Bearer 8f4259da698c2bf4391bdbe9fcac33dfa2cc9a31c0777b6f55e109327697adc9
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
    "bookmarkable_id": 67,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/67/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f4259da698c2bf4391bdbe9fcac33dfa2cc9a31c0777b6f55e109327697adc9"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/45/votes
Content-Type: application/json
Authorization: Bearer 8c5d3aee5ee222754f6db19d583b8eefcd53a382512ffe186b42b1f59543087b
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 45,
    "user_id": 405
  }
}
```



```shell
curl "api.goskive.com/v2/questions/45/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c5d3aee5ee222754f6db19d583b8eefcd53a382512ffe186b42b1f59543087b"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/8
Content-Type: application/json
Authorization: Bearer 5097493c9009ee734f009cfec5e563a8e524412d65c6166a708d7ffe720fded8
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
    "votable_id": 6,
    "user_id": 112
  }
}
```



```shell
curl "api.goskive.com/v2/votes/8" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5097493c9009ee734f009cfec5e563a8e524412d65c6166a708d7ffe720fded8"
```
