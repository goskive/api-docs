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
Authorization: Bearer 1052320c4066e98122fcca9d30c1da2f53b6a1911f3ea06a6ef443c34ec645bb
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
	-H "Authorization: Bearer 1052320c4066e98122fcca9d30c1da2f53b6a1911f3ea06a6ef443c34ec645bb"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a7c0cd760a46885ccdee1a9386f855882b0e9a15b90e1928e4cd3ae52d160a52
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":119,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":119,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7c0cd760a46885ccdee1a9386f855882b0e9a15b90e1928e4cd3ae52d160a52"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b3bf51680e482e7813e36cbf4377068a4e840f289df859c43914bc8c2af6933a
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":120,"pinned":true}}
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
    "id": 3,
    "course_id": 120,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T19:31:47.097Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:31:47.089Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":120,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3bf51680e482e7813e36cbf4377068a4e840f289df859c43914bc8c2af6933a"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/1/bookmarks
Content-Type: application/json
Authorization: Bearer 0ecb4e433b19b4c5ecdd9395f8f884a52f102b981fe05c265580ae06917ed074
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
    "id": 1,
    "bookmarkable_id": 1,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ecb4e433b19b4c5ecdd9395f8f884a52f102b981fe05c265580ae06917ed074"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/8/votes
Content-Type: application/json
Authorization: Bearer 5ec424041442c45405011e86601944605def82e51ebd43173cada18cfed97893
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 8,
    "user_id": 233
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ec424041442c45405011e86601944605def82e51ebd43173cada18cfed97893"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/18/bookmarks
Content-Type: application/json
Authorization: Bearer 9ecffdde66f213d7e2fe2e0a7a242079746f712d5963189964bbab02eeaac1dc
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
    "id": 3,
    "bookmarkable_id": 18,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/18/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ecffdde66f213d7e2fe2e0a7a242079746f712d5963189964bbab02eeaac1dc"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/14/votes
Content-Type: application/json
Authorization: Bearer a1d43db621bf20b4d627c4ffbd9c5784d10a3db8cb2e781b2c31703a5a7aa617
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
    "votable_id": 14,
    "user_id": 80
  }
}
```



```shell
curl "api.goskive.com/v2/questions/14/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1d43db621bf20b4d627c4ffbd9c5784d10a3db8cb2e781b2c31703a5a7aa617"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/12
Content-Type: application/json
Authorization: Bearer 268a1bf6185b5b84013dfd5b4d226d6f9977a9dc3dd1d46cde7599b26a8d9758
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
    "votable_id": 24,
    "user_id": 257
  }
}
```



```shell
curl "api.goskive.com/v2/votes/12" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 268a1bf6185b5b84013dfd5b4d226d6f9977a9dc3dd1d46cde7599b26a8d9758"
```
