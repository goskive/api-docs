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
DELETE /v2/bookmarks/10
Content-Type: application/json
Authorization: Bearer c57683700483e5bb5a86788eeb80aa235fe560f53558dfb4ce080de305daae84
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c57683700483e5bb5a86788eeb80aa235fe560f53558dfb4ce080de305daae84"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2045b032e2e1b3e714315d806a8cdf5653bf90a2a238febacb7cbfa48be99422
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
	-H "Authorization: Bearer 2045b032e2e1b3e714315d806a8cdf5653bf90a2a238febacb7cbfa48be99422"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f10dbba2c3c400933018457783697faa20448fcae96d02fcf361443588d4efc3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":56,"pinned":true}}
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
    "course_id": 56,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-18T11:41:44.723Z",
    "course_published": true,
    "updated_at": "2016-11-18T11:41:44.715Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":56,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f10dbba2c3c400933018457783697faa20448fcae96d02fcf361443588d4efc3"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/5/bookmarks
Content-Type: application/json
Authorization: Bearer 965175395335d374dd41bd960bdfe8ae30f867186c0b466da433f84de9ccf819
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
    "bookmarkable_id": 5,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 965175395335d374dd41bd960bdfe8ae30f867186c0b466da433f84de9ccf819"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/77/votes
Content-Type: application/json
Authorization: Bearer 83590d649470d9b05c49ff229029d07ac7a70ce47f3c7af41f8fc9e63ccb390c
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 77,
    "user_id": 653
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/77/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83590d649470d9b05c49ff229029d07ac7a70ce47f3c7af41f8fc9e63ccb390c"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/107/bookmarks
Content-Type: application/json
Authorization: Bearer 9c56415f55593880b598afa08aff74d34eecd73d583d2a961b53db931bbdff84
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
    "id": 9,
    "bookmarkable_id": 107,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/107/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c56415f55593880b598afa08aff74d34eecd73d583d2a961b53db931bbdff84"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/29/votes
Content-Type: application/json
Authorization: Bearer d6017374b40e575ac632977bebddbc831185654cea05174e1c2fc51202b2e859
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
    "votable_id": 29,
    "user_id": 142
  }
}
```



```shell
curl "api.goskive.com/v2/questions/29/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6017374b40e575ac632977bebddbc831185654cea05174e1c2fc51202b2e859"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/18
Content-Type: application/json
Authorization: Bearer 83929c8be58a4b8773ca65dd77cf4714f21394a2a6d6c0a49cc20f2f22c707b5
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 109,
    "user_id": 645
  }
}
```



```shell
curl "api.goskive.com/v2/votes/18" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83929c8be58a4b8773ca65dd77cf4714f21394a2a6d6c0a49cc20f2f22c707b5"
```
