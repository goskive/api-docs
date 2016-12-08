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
DELETE /v2/bookmarks/8
Content-Type: application/json
Authorization: Bearer 30f5d8f83a8991da1dabd0e3c720fabc4172cf94a1916b7abc84a6ff94026d0d
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30f5d8f83a8991da1dabd0e3c720fabc4172cf94a1916b7abc84a6ff94026d0d"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 34d839e61b7adf24a3c2019c9eac0ff46f700e12700925864fe942a9213f120a
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":57,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":57,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34d839e61b7adf24a3c2019c9eac0ff46f700e12700925864fe942a9213f120a"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 62e702cd5148d0713b39097804ec4286b73bb3327f2c6f3451fd4d059663cfd6
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":58,"pinned":true}}
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
    "course_id": 58,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T18:26:59.084Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:26:59.079Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":58,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62e702cd5148d0713b39097804ec4286b73bb3327f2c6f3451fd4d059663cfd6"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/27/bookmarks
Content-Type: application/json
Authorization: Bearer 840e67de4d07a042fe628f7f87061789fa1b18ce6ffe47588c46a0a05db8aaae
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
    "id": 5,
    "bookmarkable_id": 27,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 840e67de4d07a042fe628f7f87061789fa1b18ce6ffe47588c46a0a05db8aaae"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/60/votes
Content-Type: application/json
Authorization: Bearer 48b537aedd50035f081fdb9664400bd1aad3d339bf15ca289a5129cc35ab7675
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 60,
    "user_id": 515
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/60/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48b537aedd50035f081fdb9664400bd1aad3d339bf15ca289a5129cc35ab7675"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/37/bookmarks
Content-Type: application/json
Authorization: Bearer f21c040482b12745ddc021daca6b35d617f7d6ce01105d9d21498f2f02fd86ae
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
    "id": 4,
    "bookmarkable_id": 37,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/37/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f21c040482b12745ddc021daca6b35d617f7d6ce01105d9d21498f2f02fd86ae"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/44/votes
Content-Type: application/json
Authorization: Bearer fd4f4dad02ddc32ba7b5e39fb91c24bbfa1fda800730fec5ebbfac1a8f3504fc
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
    "votable_id": 44,
    "user_id": 148
  }
}
```



```shell
curl "api.goskive.com/v2/questions/44/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd4f4dad02ddc32ba7b5e39fb91c24bbfa1fda800730fec5ebbfac1a8f3504fc"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/21
Content-Type: application/json
Authorization: Bearer b80438fe84f0fc4a0ebb0827b9768f4d156938d3be26c6bacd148c4315395697
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
    "id": 21,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 106,
    "user_id": 840
  }
}
```



```shell
curl "api.goskive.com/v2/votes/21" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b80438fe84f0fc4a0ebb0827b9768f4d156938d3be26c6bacd148c4315395697"
```
