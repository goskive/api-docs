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
Authorization: Bearer 99f53e8f177b4d08ddb968bbf5560d3e27df472d6b4228813bc63d9e24800793
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
	-H "Authorization: Bearer 99f53e8f177b4d08ddb968bbf5560d3e27df472d6b4228813bc63d9e24800793"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0ea9195a9478c08673ed3d9315d57a953bada1e746e0547696298077f920f072
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":232,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":232,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ea9195a9478c08673ed3d9315d57a953bada1e746e0547696298077f920f072"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0c1b1ecf18bd07c5d4c6185046fb2f4b3159a9ab41f2a7dd4dab6595fe77cfee
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":233,"pinned":true}}
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
    "course_id": 233,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T13:15:26.081Z",
    "course_published": true,
    "updated_at": "2016-10-19T13:15:26.071Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":233,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c1b1ecf18bd07c5d4c6185046fb2f4b3159a9ab41f2a7dd4dab6595fe77cfee"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/36/bookmarks
Content-Type: application/json
Authorization: Bearer e1f3c7aa31785cc5f2f747435c72cfd7d7fdf2008f62fb37aa1180bb8d5934dc
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
    "id": 4,
    "bookmarkable_id": 36,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1f3c7aa31785cc5f2f747435c72cfd7d7fdf2008f62fb37aa1180bb8d5934dc"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/95/votes
Content-Type: application/json
Authorization: Bearer e0f2c05c70b7e7684800a6677c9e01646fb4bc68ca245ff148923413a7b3deeb
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
    "user_id": 967
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0f2c05c70b7e7684800a6677c9e01646fb4bc68ca245ff148923413a7b3deeb"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/87/bookmarks
Content-Type: application/json
Authorization: Bearer a8e05ec22ac3bc356607adeff86ce114ed20e2aff0b60199ef621dd72a397291
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
    "bookmarkable_id": 87,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/87/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8e05ec22ac3bc356607adeff86ce114ed20e2aff0b60199ef621dd72a397291"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/61/votes
Content-Type: application/json
Authorization: Bearer 506168541f91e91caaae38aa56c1a6e83a99abf9ce89c9a68eaee522c33d21eb
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 61,
    "user_id": 345
  }
}
```



```shell
curl "api.goskive.com/v2/questions/61/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 506168541f91e91caaae38aa56c1a6e83a99abf9ce89c9a68eaee522c33d21eb"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/15
Content-Type: application/json
Authorization: Bearer a392353dd43420709d0307d660f894b8802d2eddf09c9ee37dc3aaed80113281
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 89,
    "user_id": 717
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a392353dd43420709d0307d660f894b8802d2eddf09c9ee37dc3aaed80113281"
```
