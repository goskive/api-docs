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
Authorization: Bearer d179ccd6c0668186ea729abaed6e55dcffb3c47a82ca928dce3d5d2f19712d3e
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
	-H "Authorization: Bearer d179ccd6c0668186ea729abaed6e55dcffb3c47a82ca928dce3d5d2f19712d3e"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 62b10ff6260934a8fd65e071e91eed1cdbdbba15d84f04f1a883393238b44c2b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":104,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":104,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62b10ff6260934a8fd65e071e91eed1cdbdbba15d84f04f1a883393238b44c2b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 016fb816240a1a29511245f1842ad16f5e34243e8244a7923fbc2391a7f20c83
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":105,"pinned":true}}
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
    "id": 6,
    "course_id": 105,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T21:04:32.691Z",
    "course_published": true,
    "updated_at": "2016-12-08T21:04:32.686Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":105,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 016fb816240a1a29511245f1842ad16f5e34243e8244a7923fbc2391a7f20c83"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/79/bookmarks
Content-Type: application/json
Authorization: Bearer d96f4fc17bd8f37e64b07b698949f7baa1b60e25a432d940ba62d85b25c6fd03
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
    "bookmarkable_id": 79,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/79/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d96f4fc17bd8f37e64b07b698949f7baa1b60e25a432d940ba62d85b25c6fd03"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/31/votes
Content-Type: application/json
Authorization: Bearer 1005a8bd021bb8f4bb45273d4e5b441babc27a3c108a53f971847cb4c31ad155
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
    "votable_id": 31,
    "user_id": 182
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/31/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1005a8bd021bb8f4bb45273d4e5b441babc27a3c108a53f971847cb4c31ad155"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/55/bookmarks
Content-Type: application/json
Authorization: Bearer ea8b29ad9021582c92dd4159025c4a4105b3439d9c6cf1fca3052f3d410032fc
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
    "id": 2,
    "bookmarkable_id": 55,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/55/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea8b29ad9021582c92dd4159025c4a4105b3439d9c6cf1fca3052f3d410032fc"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/58/votes
Content-Type: application/json
Authorization: Bearer a1c24728b280bf9f40d57a3dd59d0cb563a353fb68e086d17817db070d0cbdc2
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
    "votable_id": 58,
    "user_id": 206
  }
}
```



```shell
curl "api.goskive.com/v2/questions/58/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1c24728b280bf9f40d57a3dd59d0cb563a353fb68e086d17817db070d0cbdc2"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/22
Content-Type: application/json
Authorization: Bearer 976a37a25c11149a106c2f0c257c8d8fbee8b9696404b3fbd600b4b60bc96d86
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
    "votable_id": 133,
    "user_id": 978
  }
}
```



```shell
curl "api.goskive.com/v2/votes/22" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 976a37a25c11149a106c2f0c257c8d8fbee8b9696404b3fbd600b4b60bc96d86"
```
