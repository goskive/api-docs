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
DELETE /v2/bookmarks/3
Content-Type: application/json
Authorization: Bearer 5811ad96865fd386a948e4c51dfc1d6dabf31ba39e10f252330a25ee1e2df1a5
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5811ad96865fd386a948e4c51dfc1d6dabf31ba39e10f252330a25ee1e2df1a5"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 09daaefa987bafc5eb2f25f5e00ac8f09f6aba7186395dfc5709e696ff305d1b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":42,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":42,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09daaefa987bafc5eb2f25f5e00ac8f09f6aba7186395dfc5709e696ff305d1b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3f5a74b0149a70614e0acae151fee3873bf2bdf4cac88be2c161b456d8723398
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
201 Created
```


```json
{
  "user_course": {
    "id": 4,
    "course_id": 41,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-20T09:45:54.791Z",
    "course_published": true,
    "updated_at": "2016-10-20T09:45:54.782Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":41,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f5a74b0149a70614e0acae151fee3873bf2bdf4cac88be2c161b456d8723398"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/69/bookmarks
Content-Type: application/json
Authorization: Bearer 543c8b1e42ca72d30b78e3d780c0f5af43d9fd2a32f6871eab77f4c824d9d451
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
    "bookmarkable_id": 69,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/69/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 543c8b1e42ca72d30b78e3d780c0f5af43d9fd2a32f6871eab77f4c824d9d451"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/43/votes
Content-Type: application/json
Authorization: Bearer 91c829744fca995449f5772c32895d7cca657d5b405919845b991b3adf885a73
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
    "id": 3,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 43,
    "user_id": 419
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91c829744fca995449f5772c32895d7cca657d5b405919845b991b3adf885a73"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/46/bookmarks
Content-Type: application/json
Authorization: Bearer 126257f8fe6acb9d18f1b88e025118fbdd42f8b1cccfee58d70942be8befb9f0
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
    "bookmarkable_id": 46,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/46/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 126257f8fe6acb9d18f1b88e025118fbdd42f8b1cccfee58d70942be8befb9f0"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/77/votes
Content-Type: application/json
Authorization: Bearer 4fc8b3df5ae27566245090845f1f9c4025a4a29eeea9f42aa240494626b577bd
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
    "id": 17,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 77,
    "user_id": 783
  }
}
```



```shell
curl "api.goskive.com/v2/questions/77/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fc8b3df5ae27566245090845f1f9c4025a4a29eeea9f42aa240494626b577bd"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/20
Content-Type: application/json
Authorization: Bearer 5c2df6f6d69912c31a67c9f428d6bf822f695f9865fe61866b7fea807dce4d8c
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 132,
    "user_id": 948
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c2df6f6d69912c31a67c9f428d6bf822f695f9865fe61866b7fea807dce4d8c"
```
