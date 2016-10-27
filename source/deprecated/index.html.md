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
Authorization: Bearer 03613416552f5692cddd9d14ff29e773ceadd8fb29582c97a4b5373efdb1cbf1
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
	-H "Authorization: Bearer 03613416552f5692cddd9d14ff29e773ceadd8fb29582c97a4b5373efdb1cbf1"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer aa26e2d25f2f16dee2dd723d1e3ce57acf06115bee249895eefd155a29dc6df1
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":294,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":294,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa26e2d25f2f16dee2dd723d1e3ce57acf06115bee249895eefd155a29dc6df1"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f67749d32d70020d21eae1e3e6d4297cf390df030547831b22cb5f90328725a4
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":293,"pinned":true}}
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
    "course_id": 293,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T17:34:51.111Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:34:51.103Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":293,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f67749d32d70020d21eae1e3e6d4297cf390df030547831b22cb5f90328725a4"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer d1f742ad91058166560e0b78432df524f7da46e7d1fe2e60671d54c2226a41f9
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
    "id": 10,
    "bookmarkable_id": 95,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1f742ad91058166560e0b78432df524f7da46e7d1fe2e60671d54c2226a41f9"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/17/votes
Content-Type: application/json
Authorization: Bearer 0258f79e7d415ea653021abdb4233fde66c99a500f627ca5351ba7f666252570
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
    "votable_id": 17,
    "user_id": 357
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/17/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0258f79e7d415ea653021abdb4233fde66c99a500f627ca5351ba7f666252570"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/125/bookmarks
Content-Type: application/json
Authorization: Bearer b2c661747169a678fcc244cf6021c9f9423e9937a2ee3b4ddcefb37d7a3daeba
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
    "bookmarkable_id": 125,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/125/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2c661747169a678fcc244cf6021c9f9423e9937a2ee3b4ddcefb37d7a3daeba"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/96/votes
Content-Type: application/json
Authorization: Bearer f5554f9eb4da6c347e20e93884c443d82c1242aaf03f2b14f2a979683c9a4da8
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 96,
    "user_id": 839
  }
}
```



```shell
curl "api.goskive.com/v2/questions/96/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5554f9eb4da6c347e20e93884c443d82c1242aaf03f2b14f2a979683c9a4da8"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/23
Content-Type: application/json
Authorization: Bearer e3d3f631cac861034157f26bc30f800dd9ec4119194050ea77a211f820042e18
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 134,
    "user_id": 979
  }
}
```



```shell
curl "api.goskive.com/v2/votes/23" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3d3f631cac861034157f26bc30f800dd9ec4119194050ea77a211f820042e18"
```
