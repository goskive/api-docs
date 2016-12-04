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
Authorization: Bearer 3b93b8b98f553d1d45ef59debe6a5cdfd07c4c8395d85f1fce9b06088cff613f
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
	-H "Authorization: Bearer 3b93b8b98f553d1d45ef59debe6a5cdfd07c4c8395d85f1fce9b06088cff613f"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a2927bd6c52a08945be6eb4d2210372a9fa6ed2ed81cecc2738e3c9939378fc2
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":161,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":161,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2927bd6c52a08945be6eb4d2210372a9fa6ed2ed81cecc2738e3c9939378fc2"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f7ad0e19cf27cf92dac5ff9495b93630ebf91b43e81ada61bc825d37cbc80f08
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":162,"pinned":true}}
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
    "id": 7,
    "course_id": 162,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-04T11:15:42.825Z",
    "course_published": true,
    "updated_at": "2016-12-04T11:15:42.817Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":162,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7ad0e19cf27cf92dac5ff9495b93630ebf91b43e81ada61bc825d37cbc80f08"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/57/bookmarks
Content-Type: application/json
Authorization: Bearer e4a817800f2dd8bf2f016b1be3079800e519f16aeeedb8ad5eab0bfad0cf9858
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
    "bookmarkable_id": 57,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4a817800f2dd8bf2f016b1be3079800e519f16aeeedb8ad5eab0bfad0cf9858"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/50/votes
Content-Type: application/json
Authorization: Bearer 0b9213a6eb3abedcd88ba5d21f98af2d45d1b7c6fcf24554cf2766a395adcac8
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 50,
    "user_id": 487
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b9213a6eb3abedcd88ba5d21f98af2d45d1b7c6fcf24554cf2766a395adcac8"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/79/bookmarks
Content-Type: application/json
Authorization: Bearer 5ad854159961c162ab42abe63fadb53c4a213a4bdadf044c964fc75730f6a57f
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
    "bookmarkable_id": 79,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/79/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ad854159961c162ab42abe63fadb53c4a213a4bdadf044c964fc75730f6a57f"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/92/votes
Content-Type: application/json
Authorization: Bearer 1fda4d9e34671fbdd30dc467fdfbd9eea7da72018743664a2d2552cc11cd247f
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 92,
    "user_id": 765
  }
}
```



```shell
curl "api.goskive.com/v2/questions/92/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fda4d9e34671fbdd30dc467fdfbd9eea7da72018743664a2d2552cc11cd247f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/10
Content-Type: application/json
Authorization: Bearer 44dde409c4077b8ad533c0dbad1aa2140fbc9daf6c02d84dbc58955151a3b4d5
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 77,
    "user_id": 564
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44dde409c4077b8ad533c0dbad1aa2140fbc9daf6c02d84dbc58955151a3b4d5"
```
