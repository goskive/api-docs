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
DELETE /v2/bookmarks/3
Content-Type: application/json
Authorization: Bearer c14cf3de0805062e088524e3d6e64b877fdc25796556631ceb8eb9b2c65ea9bf
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
	-H "Authorization: Bearer c14cf3de0805062e088524e3d6e64b877fdc25796556631ceb8eb9b2c65ea9bf"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a11d2913b1d6f40ffc0a6c6e241638ab04bba9d9ee5635f2d0b5582115032221
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":51,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":51,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a11d2913b1d6f40ffc0a6c6e241638ab04bba9d9ee5635f2d0b5582115032221"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8af201de12e8737e66302f1a985a8827937d2e903e6aa0a4b29c009178f2ac37
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":52,"pinned":true}}
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
    "course_id": 52,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T19:21:11.268Z",
    "course_published": true,
    "updated_at": "2016-12-15T19:21:11.261Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":52,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8af201de12e8737e66302f1a985a8827937d2e903e6aa0a4b29c009178f2ac37"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/1/bookmarks
Content-Type: application/json
Authorization: Bearer 92bc19939b59e31309d82e1a4f52948491ad2ef25bff5085e0c313dede5991a8
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
    "id": 1,
    "bookmarkable_id": 1,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92bc19939b59e31309d82e1a4f52948491ad2ef25bff5085e0c313dede5991a8"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/38/votes
Content-Type: application/json
Authorization: Bearer 510b8f8214edd433788e47998c33f4d23a3c6fa25c82774fa689dde996c769c9
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 38,
    "user_id": 458
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/38/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 510b8f8214edd433788e47998c33f4d23a3c6fa25c82774fa689dde996c769c9"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/30/bookmarks
Content-Type: application/json
Authorization: Bearer e8d3fa0d6f31235bfbb6bb2f13520d663fad726dfbe0843ca3e5251496925456
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
    "id": 5,
    "bookmarkable_id": 30,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/30/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8d3fa0d6f31235bfbb6bb2f13520d663fad726dfbe0843ca3e5251496925456"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/36/votes
Content-Type: application/json
Authorization: Bearer bf08d657029d4791e5695ac84d74303e335bbee56a28fd165269ee1753cbb80f
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 36,
    "user_id": 487
  }
}
```



```shell
curl "api.goskive.com/v2/questions/36/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf08d657029d4791e5695ac84d74303e335bbee56a28fd165269ee1753cbb80f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/19
Content-Type: application/json
Authorization: Bearer 269709bd4ea307c0406011498744449d663e5c4948504592a023eb2a0cdf59b8
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 99,
    "user_id": 809
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 269709bd4ea307c0406011498744449d663e5c4948504592a023eb2a0cdf59b8"
```
