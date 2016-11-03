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
DELETE /v2/bookmarks/9
Content-Type: application/json
Authorization: Bearer c53acad2964e30be58ca2f5e120b694c61c1edde84e236beb641623d1e7c64f7
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c53acad2964e30be58ca2f5e120b694c61c1edde84e236beb641623d1e7c64f7"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9c9275ea5dd64dad64ac61417708fc667b5583d288b260cd186db6d849de06e7
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":41,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":41,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c9275ea5dd64dad64ac61417708fc667b5583d288b260cd186db6d849de06e7"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2cfbda69989ec8bafa46fac3af8ad8b126bd9d3a32bfd3fab0233a9f1d77c48e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":40,"pinned":true}}
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
    "course_id": 40,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T12:33:37.140Z",
    "course_published": true,
    "updated_at": "2016-11-03T12:33:37.133Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":40,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cfbda69989ec8bafa46fac3af8ad8b126bd9d3a32bfd3fab0233a9f1d77c48e"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/10/bookmarks
Content-Type: application/json
Authorization: Bearer 7f6edd84c12958e289e6094474cce347038bdcc4518bf3b9a90e3023c31811bb
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
    "id": 2,
    "bookmarkable_id": 10,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/10/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f6edd84c12958e289e6094474cce347038bdcc4518bf3b9a90e3023c31811bb"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/87/votes
Content-Type: application/json
Authorization: Bearer 4c1073dd74641a2dda70bd80dfdf08fdadf55c36f374ecb459025d830dca332d
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 87,
    "user_id": 903
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c1073dd74641a2dda70bd80dfdf08fdadf55c36f374ecb459025d830dca332d"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/98/bookmarks
Content-Type: application/json
Authorization: Bearer 6b384a58a63fc2fbff4efef8e25e589acff2d8cf1b7afe0a7738022de07270a1
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
    "id": 10,
    "bookmarkable_id": 98,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/98/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b384a58a63fc2fbff4efef8e25e589acff2d8cf1b7afe0a7738022de07270a1"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/20/votes
Content-Type: application/json
Authorization: Bearer b6e07aac615e46ba8567619495dd70663e3a2ca04612cb07722d8d986dbf7845
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
    "votable_id": 20,
    "user_id": 163
  }
}
```



```shell
curl "api.goskive.com/v2/questions/20/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6e07aac615e46ba8567619495dd70663e3a2ca04612cb07722d8d986dbf7845"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/12
Content-Type: application/json
Authorization: Bearer 1bde8812c8c9feeeb8610e2a9407bc28676d402ba6aadb742d6080f308126ee8
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
    "votable_id": 53,
    "user_id": 370
  }
}
```



```shell
curl "api.goskive.com/v2/votes/12" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bde8812c8c9feeeb8610e2a9407bc28676d402ba6aadb742d6080f308126ee8"
```
