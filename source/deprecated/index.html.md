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
Authorization: Bearer 346bea71016905a934e00c1d1134932d683858198762b95de9f2d4942d5b2e2b
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
	-H "Authorization: Bearer 346bea71016905a934e00c1d1134932d683858198762b95de9f2d4942d5b2e2b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b9bd7b30b92c1cd7b4bcec4e1508ba66bae3297527e083d36fa62eafeaa71b80
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":97,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":97,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9bd7b30b92c1cd7b4bcec4e1508ba66bae3297527e083d36fa62eafeaa71b80"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7445453bb177d1a7286c2dd6218a2bf46ec00fc8638548984c2066dd0dbb03d9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":98,"pinned":true}}
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
    "course_id": 98,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T18:09:41.313Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:09:41.308Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":98,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7445453bb177d1a7286c2dd6218a2bf46ec00fc8638548984c2066dd0dbb03d9"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/77/bookmarks
Content-Type: application/json
Authorization: Bearer 8e505c5e11235b6992fd02e8de6915c51b09ea05d3140487c7817f12137bd973
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
    "bookmarkable_id": 77,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/77/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e505c5e11235b6992fd02e8de6915c51b09ea05d3140487c7817f12137bd973"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/95/votes
Content-Type: application/json
Authorization: Bearer bae0a6d170041c8a2f2c4df703ff5149a6ca456f094992a406de644312d691f5
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 95,
    "user_id": 947
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bae0a6d170041c8a2f2c4df703ff5149a6ca456f094992a406de644312d691f5"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/133/bookmarks
Content-Type: application/json
Authorization: Bearer f901eed8d565083fae5a33b6507197d4bb0f61aca6954973de479309c9111f8e
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
    "bookmarkable_id": 133,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/133/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f901eed8d565083fae5a33b6507197d4bb0f61aca6954973de479309c9111f8e"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/132/votes
Content-Type: application/json
Authorization: Bearer cd2a46578da50f43985e3a0f3e9c6c28a8853af49884f7212ea2174a534861a6
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 132,
    "user_id": 973
  }
}
```



```shell
curl "api.goskive.com/v2/questions/132/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd2a46578da50f43985e3a0f3e9c6c28a8853af49884f7212ea2174a534861a6"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/7
Content-Type: application/json
Authorization: Bearer 4aa6e2c97a3d7189865809d0c87f100f9ae3aebac90f59d225b21cb321844378
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 113,
    "user_id": 785
  }
}
```



```shell
curl "api.goskive.com/v2/votes/7" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4aa6e2c97a3d7189865809d0c87f100f9ae3aebac90f59d225b21cb321844378"
```
