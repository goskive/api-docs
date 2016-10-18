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
DELETE /v2/bookmarks/1
Content-Type: application/json
Authorization: Bearer 28ae60fcd647ad75c8720be1fccc43e2c4ebfdd814c39ec6dcf9435c7ec79f57
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28ae60fcd647ad75c8720be1fccc43e2c4ebfdd814c39ec6dcf9435c7ec79f57"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer bea39c356722cbc1da085102f26179b59083f93f058465f2f21d45daf425957e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":223,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":223,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bea39c356722cbc1da085102f26179b59083f93f058465f2f21d45daf425957e"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f91f5a9098c7131f8047d241c30d974f2256fccbd92d621b7cf8fa4ee74e253c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":224,"pinned":true}}
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
    "id": 2,
    "course_id": 224,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T09:28:41.170Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:28:41.160Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":224,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f91f5a9098c7131f8047d241c30d974f2256fccbd92d621b7cf8fa4ee74e253c"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/92/bookmarks
Content-Type: application/json
Authorization: Bearer 4f12ff0b6997c19010e470d0a7c4f4fcc1681e558b07a20d7b95cac12c3bf0ec
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
    "bookmarkable_id": 92,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/92/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f12ff0b6997c19010e470d0a7c4f4fcc1681e558b07a20d7b95cac12c3bf0ec"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/1/votes
Content-Type: application/json
Authorization: Bearer cf94e91778552627ea263293436e0c457edca886a4d69aa67bab80b065b55d60
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 1,
    "user_id": 5
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf94e91778552627ea263293436e0c457edca886a4d69aa67bab80b065b55d60"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/134/bookmarks
Content-Type: application/json
Authorization: Bearer 628bf72b93eac324e5914eafcf08f985f358f626cc74cd97c82fc91630853f80
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
    "bookmarkable_id": 134,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 628bf72b93eac324e5914eafcf08f985f358f626cc74cd97c82fc91630853f80"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/8/votes
Content-Type: application/json
Authorization: Bearer 266494a4e49f1b43acb74ba8b6b02a192ddd6f7bd8c45e43102dc1b97c9d1a2f
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
    "votable_id": 8,
    "user_id": 95
  }
}
```



```shell
curl "api.goskive.com/v2/questions/8/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 266494a4e49f1b43acb74ba8b6b02a192ddd6f7bd8c45e43102dc1b97c9d1a2f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/11
Content-Type: application/json
Authorization: Bearer bb0646d8bc21e3e834350b6255b5c7c145ed39a103fce17014760949b0027dfe
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 11,
    "user_id": 202
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb0646d8bc21e3e834350b6255b5c7c145ed39a103fce17014760949b0027dfe"
```
