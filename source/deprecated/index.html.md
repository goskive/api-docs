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
DELETE /v2/bookmarks/6
Content-Type: application/json
Authorization: Bearer 13bfb528bbf5f8cecad786997174732a1ab55c6d7a86e3d5cd0957a32bb9522d
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13bfb528bbf5f8cecad786997174732a1ab55c6d7a86e3d5cd0957a32bb9522d"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 815567d94e7b1254d65d77a76e0c9d0b08e6e2ca92f5133040d335731a5a888c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":157,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":157,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 815567d94e7b1254d65d77a76e0c9d0b08e6e2ca92f5133040d335731a5a888c"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c89575b7b4b7ab36db263d551f075fb0090865d9ddc62f5976c700154ca4db1d
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":158,"pinned":true}}
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
    "course_id": 158,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-21T15:04:17.938Z",
    "course_published": true,
    "updated_at": "2016-10-21T15:04:17.929Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":158,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c89575b7b4b7ab36db263d551f075fb0090865d9ddc62f5976c700154ca4db1d"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/79/bookmarks
Content-Type: application/json
Authorization: Bearer 401d0f4aaa03d1ab9c3aa039cbfb0461accc8b6337f2bb637feae02aa9830c98
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
    "bookmarkable_id": 79,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/79/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 401d0f4aaa03d1ab9c3aa039cbfb0461accc8b6337f2bb637feae02aa9830c98"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/93/votes
Content-Type: application/json
Authorization: Bearer 6ae1d1d4aa71ff37e5e362a7102a046b90ecf58e0845774511e7b05d7ddc4639
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
    "votable_id": 93,
    "user_id": 958
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/93/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ae1d1d4aa71ff37e5e362a7102a046b90ecf58e0845774511e7b05d7ddc4639"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/132/bookmarks
Content-Type: application/json
Authorization: Bearer 411b0d61e7d13bee5c0b8c8d83243c943cf2aa0030dcb47f50f325a5e99419f6
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
    "bookmarkable_id": 132,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/132/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 411b0d61e7d13bee5c0b8c8d83243c943cf2aa0030dcb47f50f325a5e99419f6"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/55/votes
Content-Type: application/json
Authorization: Bearer 8839e16a63f8b39718331173820bd41aadbcc42cab63f39c780ba7b0bbdd295f
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
    "votable_id": 55,
    "user_id": 214
  }
}
```



```shell
curl "api.goskive.com/v2/questions/55/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8839e16a63f8b39718331173820bd41aadbcc42cab63f39c780ba7b0bbdd295f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/13
Content-Type: application/json
Authorization: Bearer a75a65dd6b817fd3418b759b7c6cca098b08b6904f160973608bd6bff3e3f450
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 123,
    "user_id": 848
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a75a65dd6b817fd3418b759b7c6cca098b08b6904f160973608bd6bff3e3f450"
```
