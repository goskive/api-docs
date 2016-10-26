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
Authorization: Bearer 7842faeaa1665760adfe9aa8fec21c379b09af4231efaf1cae84ba70bf972be3
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
	-H "Authorization: Bearer 7842faeaa1665760adfe9aa8fec21c379b09af4231efaf1cae84ba70bf972be3"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9e6dd0fcd066bf6723a79728bb336522b06558b6891fc0ae9430e1a92d4d898b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":134,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":134,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e6dd0fcd066bf6723a79728bb336522b06558b6891fc0ae9430e1a92d4d898b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 28ba94ea3ff515d73a9fe089a2e2046cc380c73dc2dc2f6e57e9a4c2c4b8d235
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":135,"pinned":true}}
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
    "course_id": 135,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T18:00:55.490Z",
    "course_published": true,
    "updated_at": "2016-10-26T18:00:55.480Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":135,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28ba94ea3ff515d73a9fe089a2e2046cc380c73dc2dc2f6e57e9a4c2c4b8d235"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/75/bookmarks
Content-Type: application/json
Authorization: Bearer 39d1895e0582e27649a7a43174639ddec31b9eb4bcbb32a3d4c079be0fb22524
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
    "bookmarkable_id": 75,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/75/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39d1895e0582e27649a7a43174639ddec31b9eb4bcbb32a3d4c079be0fb22524"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/93/votes
Content-Type: application/json
Authorization: Bearer 8dc66d9f6622708d28e16f476200dbc593c28af96d3604db96ca9feb6c1e5cfb
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
    "votable_id": 93,
    "user_id": 964
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/93/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8dc66d9f6622708d28e16f476200dbc593c28af96d3604db96ca9feb6c1e5cfb"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/41/bookmarks
Content-Type: application/json
Authorization: Bearer bcaab9661d3cf0f180557c3078b3a089bed034c6b929ed6f81cf3dac63ef2546
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
    "bookmarkable_id": 41,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/41/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcaab9661d3cf0f180557c3078b3a089bed034c6b929ed6f81cf3dac63ef2546"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/76/votes
Content-Type: application/json
Authorization: Bearer 0ba3f6b367b76240eb7de98942522ee896833c026a0485b1d1f47408ab46b43c
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 76,
    "user_id": 509
  }
}
```



```shell
curl "api.goskive.com/v2/questions/76/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ba3f6b367b76240eb7de98942522ee896833c026a0485b1d1f47408ab46b43c"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/6
Content-Type: application/json
Authorization: Bearer 86c1ec2260d645982398aa88878f06da00149a12e8481756e7896c9f711bba26
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 50,
    "user_id": 169
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86c1ec2260d645982398aa88878f06da00149a12e8481756e7896c9f711bba26"
```
