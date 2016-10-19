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
DELETE /v2/bookmarks/5
Content-Type: application/json
Authorization: Bearer ace76d0cd69fd5d9d86f04a25b13c6a0ac709f6de8ede75c0cf6803aefd57718
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ace76d0cd69fd5d9d86f04a25b13c6a0ac709f6de8ede75c0cf6803aefd57718"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7f1a68b1a953fa2b873153461c0501dd449f2692ab543224ab957a47d84d2bf6
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":154,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":154,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f1a68b1a953fa2b873153461c0501dd449f2692ab543224ab957a47d84d2bf6"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 556f2f5836ef2a976c3c528e4158d2b91226120ac3b9b9ca93bc5e202c1e2425
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":153,"pinned":true}}
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
    "course_id": 153,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T11:45:20.440Z",
    "course_published": true,
    "updated_at": "2016-10-19T11:45:20.430Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":153,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 556f2f5836ef2a976c3c528e4158d2b91226120ac3b9b9ca93bc5e202c1e2425"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer b0730988bb33ff7adda0f1837e8046b43837d7c017bcc9c9217a39b44266b312
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
    "bookmarkable_id": 95,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0730988bb33ff7adda0f1837e8046b43837d7c017bcc9c9217a39b44266b312"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/26/votes
Content-Type: application/json
Authorization: Bearer 0e21db1e6e3ae638b548840614b07c033a26419e1acf54ebc2e4ed876e804d01
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 26,
    "user_id": 473
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/26/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e21db1e6e3ae638b548840614b07c033a26419e1acf54ebc2e4ed876e804d01"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/130/bookmarks
Content-Type: application/json
Authorization: Bearer e860ac426bd0cd7e92293b51eddea926b02b93d2b2ae6b5e039e55fc114e5206
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
    "bookmarkable_id": 130,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/130/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e860ac426bd0cd7e92293b51eddea926b02b93d2b2ae6b5e039e55fc114e5206"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/97/votes
Content-Type: application/json
Authorization: Bearer f438b77ce064181e19ea2565475d22b587f57de377e160d63122d425050062a6
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
    "votable_id": 97,
    "user_id": 616
  }
}
```



```shell
curl "api.goskive.com/v2/questions/97/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f438b77ce064181e19ea2565475d22b587f57de377e160d63122d425050062a6"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/17
Content-Type: application/json
Authorization: Bearer c4052a23c05132f669b80f94a0038838aa3286083b69382834081d11b9922142
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
    "id": 17,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 128,
    "user_id": 933
  }
}
```



```shell
curl "api.goskive.com/v2/votes/17" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4052a23c05132f669b80f94a0038838aa3286083b69382834081d11b9922142"
```
