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
DELETE /v2/bookmarks/7
Content-Type: application/json
Authorization: Bearer 049329c920a16efcf9c518effcd2c1dba963f21b813ad37de3756565e072a1f4
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 049329c920a16efcf9c518effcd2c1dba963f21b813ad37de3756565e072a1f4"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7d882b5561c521dd0dc672c50d2c5959e94beff3e60b6a9eb2d7e5f742745b5d
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":315,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":315,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d882b5561c521dd0dc672c50d2c5959e94beff3e60b6a9eb2d7e5f742745b5d"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8a2b394cd5fbc5c07dc5b8b9d1250cd9e835f746457104dee1e1002501152d65
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":316,"pinned":true}}
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
    "course_id": 316,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T19:50:37.216Z",
    "course_published": true,
    "updated_at": "2016-12-15T19:50:37.212Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":316,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a2b394cd5fbc5c07dc5b8b9d1250cd9e835f746457104dee1e1002501152d65"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/33/bookmarks
Content-Type: application/json
Authorization: Bearer 32641449ddd548b0a2bf83fa96f91e3995b8428dc13465f82142afec32243b76
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
    "bookmarkable_id": 33,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32641449ddd548b0a2bf83fa96f91e3995b8428dc13465f82142afec32243b76"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/72/votes
Content-Type: application/json
Authorization: Bearer 9a0fee3de5d77989612633f6ef038c965a70cda5649f591f47117ee14e6a4871
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 72,
    "user_id": 662
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/72/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a0fee3de5d77989612633f6ef038c965a70cda5649f591f47117ee14e6a4871"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/59/bookmarks
Content-Type: application/json
Authorization: Bearer 6cf5b4a385c300f9ddc33b9f4e81f46c17b56b8eaeae3155cb98a2eca88513b1
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
    "bookmarkable_id": 59,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/59/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cf5b4a385c300f9ddc33b9f4e81f46c17b56b8eaeae3155cb98a2eca88513b1"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/111/votes
Content-Type: application/json
Authorization: Bearer 59b4f3dd1ce247e8d1635ebb656c49df11be92f3405cf62744fe6b600ae7dea5
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 111,
    "user_id": 807
  }
}
```



```shell
curl "api.goskive.com/v2/questions/111/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59b4f3dd1ce247e8d1635ebb656c49df11be92f3405cf62744fe6b600ae7dea5"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/1
Content-Type: application/json
Authorization: Bearer f63a1e77cd440c1f83762157aee0d1357b71670c8a4f537b47e9af37dd89b508
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 6,
    "user_id": 29
  }
}
```



```shell
curl "api.goskive.com/v2/votes/1" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f63a1e77cd440c1f83762157aee0d1357b71670c8a4f537b47e9af37dd89b508"
```
