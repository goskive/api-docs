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
Authorization: Bearer c0362ca73154e26b94c4ce624a83966f3eadf2ef7493c08d70669d012fb736b5
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
	-H "Authorization: Bearer c0362ca73154e26b94c4ce624a83966f3eadf2ef7493c08d70669d012fb736b5"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a6a73cd21cc5432f5c84c32d8a9d6826dc6c95190d406366f243bbd7fdffd9b4
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":199,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":199,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6a73cd21cc5432f5c84c32d8a9d6826dc6c95190d406366f243bbd7fdffd9b4"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 94c95b839c95fbe63e66fffa9ddc20a82bd9ba5f81d5409146944e8db7ed3a5c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":200,"pinned":true}}
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
    "course_id": 200,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T16:44:10.212Z",
    "course_published": true,
    "updated_at": "2016-10-18T16:44:10.203Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":200,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94c95b839c95fbe63e66fffa9ddc20a82bd9ba5f81d5409146944e8db7ed3a5c"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/27/bookmarks
Content-Type: application/json
Authorization: Bearer 60a2a682d5247b981e48c42dbdcfedec37a8bd7b4671badfe7f7ce45385157d3
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
    "bookmarkable_id": 27,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60a2a682d5247b981e48c42dbdcfedec37a8bd7b4671badfe7f7ce45385157d3"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/95/votes
Content-Type: application/json
Authorization: Bearer ef3c53b37f4a42ec1fc189ea74417eed2414054e7872eb8ec89b54754984fcb0
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
    "id": 22,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 95,
    "user_id": 964
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef3c53b37f4a42ec1fc189ea74417eed2414054e7872eb8ec89b54754984fcb0"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/5/bookmarks
Content-Type: application/json
Authorization: Bearer c5106cc6e00900bcd5433a0baa3ac78a16e50bf64067f8533a9ddae76569e67e
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
    "bookmarkable_id": 5,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/5/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5106cc6e00900bcd5433a0baa3ac78a16e50bf64067f8533a9ddae76569e67e"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/94/votes
Content-Type: application/json
Authorization: Bearer 6e055c554f2d1d99a114cad4f2fdbf5fe1b22555901a4dd72264d63a56d9320b
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 94,
    "user_id": 809
  }
}
```



```shell
curl "api.goskive.com/v2/questions/94/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e055c554f2d1d99a114cad4f2fdbf5fe1b22555901a4dd72264d63a56d9320b"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/5
Content-Type: application/json
Authorization: Bearer 229740f2f8861ac485fd85badd02d6c474e125eedd4d1b5b3447fbbd618939bb
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 33,
    "user_id": 426
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 229740f2f8861ac485fd85badd02d6c474e125eedd4d1b5b3447fbbd618939bb"
```
