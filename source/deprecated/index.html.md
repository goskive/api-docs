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
Authorization: Bearer 435e2bf2675b3c4a6d5b054c92f7a832834fb5eb41bf783643e64f7f62208a7f
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
	-H "Authorization: Bearer 435e2bf2675b3c4a6d5b054c92f7a832834fb5eb41bf783643e64f7f62208a7f"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a24c131b319c63ab42e07bfbf2b44796bb6c6e4b5b46983ddd02d6df04af1fba
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":304,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":304,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a24c131b319c63ab42e07bfbf2b44796bb6c6e4b5b46983ddd02d6df04af1fba"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9b91030389a996588b4ce684125d8d6526559b095323ea0bcd627646a673f183
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":305,"pinned":true}}
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
    "id": 6,
    "course_id": 305,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T18:22:27.677Z",
    "course_published": true,
    "updated_at": "2016-10-13T18:22:27.668Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":305,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b91030389a996588b4ce684125d8d6526559b095323ea0bcd627646a673f183"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/27/bookmarks
Content-Type: application/json
Authorization: Bearer 150cdc5f448b2bc917b1f16b7effcb494585f17fccd6d2a17e96eb0c3463a748
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
    "id": 6,
    "bookmarkable_id": 27,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 150cdc5f448b2bc917b1f16b7effcb494585f17fccd6d2a17e96eb0c3463a748"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/36/votes
Content-Type: application/json
Authorization: Bearer 4e1ac36d4b2259798c19faf93f6b4deb0ccf82fb4b0b434198f0dc2e8bd4ccce
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 36,
    "user_id": 594
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e1ac36d4b2259798c19faf93f6b4deb0ccf82fb4b0b434198f0dc2e8bd4ccce"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/31/bookmarks
Content-Type: application/json
Authorization: Bearer 727d5ff7094ef77057faa98b0c42aadbd0234c6f66b3d7b60b01f5f1f3bdf5c5
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
    "id": 4,
    "bookmarkable_id": 31,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/31/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 727d5ff7094ef77057faa98b0c42aadbd0234c6f66b3d7b60b01f5f1f3bdf5c5"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/80/votes
Content-Type: application/json
Authorization: Bearer 64d1df72660cdb586e9cbf0a561ce4a9a593204ee4cae5061e6c2e1ba0fd927e
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 80,
    "user_id": 627
  }
}
```



```shell
curl "api.goskive.com/v2/questions/80/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64d1df72660cdb586e9cbf0a561ce4a9a593204ee4cae5061e6c2e1ba0fd927e"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/16
Content-Type: application/json
Authorization: Bearer 3eb68141e9af738fa5f7eab2109db3b3265f6c2ab96457ea6fbb6310ff52af66
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
    "votable_id": 87,
    "user_id": 697
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eb68141e9af738fa5f7eab2109db3b3265f6c2ab96457ea6fbb6310ff52af66"
```
