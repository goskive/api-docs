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
Authorization: Bearer 7feacbaf3641eb89738e8b7b96beb3ddc297706ed6d4be6289e75f097f8b2db4
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
	-H "Authorization: Bearer 7feacbaf3641eb89738e8b7b96beb3ddc297706ed6d4be6289e75f097f8b2db4"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b8f29b145a90cb792929bd1d74713486832f06a2f4b58fea88929ec0f9615760
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":172,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":172,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8f29b145a90cb792929bd1d74713486832f06a2f4b58fea88929ec0f9615760"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 864d720f409123665eb49670d16e08624897aff7d2161f19593c844d930aa744
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":171,"pinned":true}}
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
    "course_id": 171,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T12:36:59.622Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:36:59.613Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":171,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 864d720f409123665eb49670d16e08624897aff7d2161f19593c844d930aa744"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/91/bookmarks
Content-Type: application/json
Authorization: Bearer c7a924ee58b66a1eab6cf1d61fe3230494f3aa18e83b00a6c8eabed81f508a1b
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
    "bookmarkable_id": 91,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7a924ee58b66a1eab6cf1d61fe3230494f3aa18e83b00a6c8eabed81f508a1b"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/3/votes
Content-Type: application/json
Authorization: Bearer 98516845cfa7314bb84ba2d3575e73fec091535d1368e8b23fd124c777e5584e
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 3,
    "user_id": 13
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98516845cfa7314bb84ba2d3575e73fec091535d1368e8b23fd124c777e5584e"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/116/bookmarks
Content-Type: application/json
Authorization: Bearer fa8e288b1884340f16d32e8217cd2eac08d15e4029db0aca93f44172a1d56a87
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
    "bookmarkable_id": 116,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/116/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa8e288b1884340f16d32e8217cd2eac08d15e4029db0aca93f44172a1d56a87"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/51/votes
Content-Type: application/json
Authorization: Bearer f16d7dfaf35a67103bed4f576cd4a67342686dd3c48177f61149dafde980fa29
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 51,
    "user_id": 382
  }
}
```



```shell
curl "api.goskive.com/v2/questions/51/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f16d7dfaf35a67103bed4f576cd4a67342686dd3c48177f61149dafde980fa29"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/12
Content-Type: application/json
Authorization: Bearer 05bca899699a14a33e056b93ddc395e11fea676be4c65d2b6c6f2c7539fee0e1
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 95,
    "user_id": 645
  }
}
```



```shell
curl "api.goskive.com/v2/votes/12" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05bca899699a14a33e056b93ddc395e11fea676be4c65d2b6c6f2c7539fee0e1"
```
