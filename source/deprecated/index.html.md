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
Authorization: Bearer d23a397770fb4cb98e6d6c299050a7f944000ec7dda07f46f115b0094514fd54
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
	-H "Authorization: Bearer d23a397770fb4cb98e6d6c299050a7f944000ec7dda07f46f115b0094514fd54"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer dd8fb11967ec316e511b14d5ead6f1f9aa6ac47a24aa8e55b5ed6e617c7bfeab
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":92,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":92,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd8fb11967ec316e511b14d5ead6f1f9aa6ac47a24aa8e55b5ed6e617c7bfeab"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6ef9aa3731b4592d7579366683f3d64c8d6e09a28332427ad22586370a694b65
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":93,"pinned":true}}
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
    "id": 3,
    "course_id": 93,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-20T19:31:43.383Z",
    "course_published": true,
    "updated_at": "2016-10-20T19:31:43.374Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":93,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ef9aa3731b4592d7579366683f3d64c8d6e09a28332427ad22586370a694b65"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/43/bookmarks
Content-Type: application/json
Authorization: Bearer bec12c3e1e4a4558392da1ddec05f269536994ae7ebe69437c155e53999d934f
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
    "bookmarkable_id": 43,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bec12c3e1e4a4558392da1ddec05f269536994ae7ebe69437c155e53999d934f"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/48/votes
Content-Type: application/json
Authorization: Bearer 843216d1e0c79c433a9a96237ae2aeaa645412487c504410ca180aa9053526db
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
    "id": 17,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 48,
    "user_id": 516
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/48/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 843216d1e0c79c433a9a96237ae2aeaa645412487c504410ca180aa9053526db"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/45/bookmarks
Content-Type: application/json
Authorization: Bearer 314192011012c2ceee9a337b59cb96a8de8d655f75187480b5f3c7bd6f56ad79
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
    "bookmarkable_id": 45,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/45/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 314192011012c2ceee9a337b59cb96a8de8d655f75187480b5f3c7bd6f56ad79"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/1/votes
Content-Type: application/json
Authorization: Bearer 97634dada1d830dcd94c894de65b78f123870abbea82217a77d7a71c0c26131a
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
    "user_id": 18
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97634dada1d830dcd94c894de65b78f123870abbea82217a77d7a71c0c26131a"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/16
Content-Type: application/json
Authorization: Bearer c8f20b1a1b0c6d458da8ee9b9c79b765fcdd20cb7ae2cda97453b5f74d9a27bb
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 58,
    "user_id": 473
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8f20b1a1b0c6d458da8ee9b9c79b765fcdd20cb7ae2cda97453b5f74d9a27bb"
```
