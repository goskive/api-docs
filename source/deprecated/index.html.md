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
DELETE /v2/bookmarks/7
Content-Type: application/json
Authorization: Bearer d808d7c06ca9b62d20f15c059eccf08bd314d487e9ce7d8f61fe6ea2684d9bfe
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
	-H "Authorization: Bearer d808d7c06ca9b62d20f15c059eccf08bd314d487e9ce7d8f61fe6ea2684d9bfe"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f3bb9fe2b480bd59030642c052326fed6596c32466560c5cbfe5720f1428549c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":312,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":312,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3bb9fe2b480bd59030642c052326fed6596c32466560c5cbfe5720f1428549c"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer bd69281cf6a7575b44bf92e5f7a097a61f9062e632b0c64eda9edf05325bc5a0
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":311,"pinned":true}}
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
    "course_id": 311,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T15:57:23.074Z",
    "course_published": true,
    "updated_at": "2016-10-27T15:57:23.065Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":311,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd69281cf6a7575b44bf92e5f7a097a61f9062e632b0c64eda9edf05325bc5a0"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/29/bookmarks
Content-Type: application/json
Authorization: Bearer 8ea0a59f903fed96b9274f7e00ad58e8e1d441fb041ae8387402b62d6de0485c
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
    "id": 3,
    "bookmarkable_id": 29,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ea0a59f903fed96b9274f7e00ad58e8e1d441fb041ae8387402b62d6de0485c"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/72/votes
Content-Type: application/json
Authorization: Bearer 61d73bb9a493a44137066ad7a4573d34588c08935537bd3638eaa6f5b6bd2743
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
    "votable_id": 72,
    "user_id": 734
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/72/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61d73bb9a493a44137066ad7a4573d34588c08935537bd3638eaa6f5b6bd2743"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/10/bookmarks
Content-Type: application/json
Authorization: Bearer 8369452eddf7f505de67b6d2d8badb6fa12bec89e8508670825c76bbb8d76cda
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
    "id": 1,
    "bookmarkable_id": 10,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/10/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8369452eddf7f505de67b6d2d8badb6fa12bec89e8508670825c76bbb8d76cda"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/107/votes
Content-Type: application/json
Authorization: Bearer 7285f782f99542b4ed0c191f290bb289c125c9bb8d6e5c500d3e470f766a7604
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 107,
    "user_id": 728
  }
}
```



```shell
curl "api.goskive.com/v2/questions/107/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7285f782f99542b4ed0c191f290bb289c125c9bb8d6e5c500d3e470f766a7604"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/16
Content-Type: application/json
Authorization: Bearer 2d2d884584a900481ecbed856bb39199320c5e9c5bd475a1b8eb49fbb798b456
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
    "votable_id": 110,
    "user_id": 754
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d2d884584a900481ecbed856bb39199320c5e9c5bd475a1b8eb49fbb798b456"
```
