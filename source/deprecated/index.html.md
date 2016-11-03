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
DELETE /v2/bookmarks/4
Content-Type: application/json
Authorization: Bearer 6b852df0cbc25bf80bf615274cef9b5f3f1145447374bc6aab82533475ba5f6b
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b852df0cbc25bf80bf615274cef9b5f3f1145447374bc6aab82533475ba5f6b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer ee3d30182702f247466fab9762d8c239285f936934fadbd585dedb9d1f316b97
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":203,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":203,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee3d30182702f247466fab9762d8c239285f936934fadbd585dedb9d1f316b97"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer cc77e5b08334a33d1f1cacc23845f1bd5e4578e77b301acc05b2e90cd690497a
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":202,"pinned":true}}
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
    "course_id": 202,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T17:37:19.452Z",
    "course_published": true,
    "updated_at": "2016-11-03T17:37:19.442Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":202,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc77e5b08334a33d1f1cacc23845f1bd5e4578e77b301acc05b2e90cd690497a"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/33/bookmarks
Content-Type: application/json
Authorization: Bearer ccfb7f7acce936a68f5b8a67cb76bbc2a50cdffc46b8a2c4aa226a61bf540398
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
    "bookmarkable_id": 33,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccfb7f7acce936a68f5b8a67cb76bbc2a50cdffc46b8a2c4aa226a61bf540398"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/76/votes
Content-Type: application/json
Authorization: Bearer 3047ccf1631b0c6464787c8e6e2e0a8320d325269ebff82863a9edbe9e7f3334
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 76,
    "user_id": 471
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/76/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3047ccf1631b0c6464787c8e6e2e0a8320d325269ebff82863a9edbe9e7f3334"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/91/bookmarks
Content-Type: application/json
Authorization: Bearer e0861c8689e3d45731e3be39256b4451c9e52db214cc7127514f05d7e7d90ee2
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
    "id": 8,
    "bookmarkable_id": 91,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0861c8689e3d45731e3be39256b4451c9e52db214cc7127514f05d7e7d90ee2"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/22/votes
Content-Type: application/json
Authorization: Bearer 474f45a3f9ac6c3ea242f806f459feda8bdbf0ab3b9e8adca0648433faf3f2ce
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 22,
    "user_id": 232
  }
}
```



```shell
curl "api.goskive.com/v2/questions/22/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 474f45a3f9ac6c3ea242f806f459feda8bdbf0ab3b9e8adca0648433faf3f2ce"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/19
Content-Type: application/json
Authorization: Bearer 30412045798ead224d3064e89ad11373936eb058b689af364f36ff5ad9e7687f
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 99,
    "user_id": 871
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30412045798ead224d3064e89ad11373936eb058b689af364f36ff5ad9e7687f"
```
