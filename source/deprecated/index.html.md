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
Authorization: Bearer a4c45eeffafb03e2f5d9ee2fec779e0dcac18a5867c0c74f485b0d372b141c11
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
	-H "Authorization: Bearer a4c45eeffafb03e2f5d9ee2fec779e0dcac18a5867c0c74f485b0d372b141c11"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2672a4fd70fdd547463cf7e0ef1abd43e8b94b4c92bf6f2f66130f074264cb4e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":249,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":249,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2672a4fd70fdd547463cf7e0ef1abd43e8b94b4c92bf6f2f66130f074264cb4e"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c86368c3bac39af3346afbc824cdc798a5743af77a3310b43d53aeacf03ef6cb
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":248,"pinned":true}}
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
    "course_id": 248,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T11:09:27.266Z",
    "course_published": true,
    "updated_at": "2016-10-18T11:09:27.257Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":248,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c86368c3bac39af3346afbc824cdc798a5743af77a3310b43d53aeacf03ef6cb"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/87/bookmarks
Content-Type: application/json
Authorization: Bearer 601a19a06d044c5c9315c4b56eb0ef09ab024b532d5155633a228b901d8124c7
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
    "id": 8,
    "bookmarkable_id": 87,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 601a19a06d044c5c9315c4b56eb0ef09ab024b532d5155633a228b901d8124c7"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/60/votes
Content-Type: application/json
Authorization: Bearer 8d36393672ea7e87fbec4bbca0fda45e28b8459d6e9bbd8262164fc50a710d84
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 60,
    "user_id": 609
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/60/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d36393672ea7e87fbec4bbca0fda45e28b8459d6e9bbd8262164fc50a710d84"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/62/bookmarks
Content-Type: application/json
Authorization: Bearer 33da11fb3409ac829b24c43556d85f8f50765d8bf1457d8f3f8604956a1e2dfd
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
    "bookmarkable_id": 62,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/62/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33da11fb3409ac829b24c43556d85f8f50765d8bf1457d8f3f8604956a1e2dfd"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/121/votes
Content-Type: application/json
Authorization: Bearer fb5787eedcc7d6053776c1d7aa5dc755e3caa8240ca52def31ee4149b3666c0d
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 121,
    "user_id": 786
  }
}
```



```shell
curl "api.goskive.com/v2/questions/121/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb5787eedcc7d6053776c1d7aa5dc755e3caa8240ca52def31ee4149b3666c0d"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/22
Content-Type: application/json
Authorization: Bearer 88b82962d78b1543709693e162cdb9c0347b7761fcda73071c69399da7a81e8a
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
    "votable_id": 126,
    "user_id": 827
  }
}
```



```shell
curl "api.goskive.com/v2/votes/22" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88b82962d78b1543709693e162cdb9c0347b7761fcda73071c69399da7a81e8a"
```
