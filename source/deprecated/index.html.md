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
Authorization: Bearer 7c7435050efab71e78cc6131b8721917cfc64b5422fa2479b1af162c07d5bc7b
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
	-H "Authorization: Bearer 7c7435050efab71e78cc6131b8721917cfc64b5422fa2479b1af162c07d5bc7b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 86325dc53790faa3c160fc717a02629f28c24d9f5afb0a66126eb385c6588950
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":253,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":253,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86325dc53790faa3c160fc717a02629f28c24d9f5afb0a66126eb385c6588950"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 677e390f79938582d90c29633a7d598ae98eaf1db72247777e6604c9be7b92d7
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":254,"pinned":true}}
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
    "id": 8,
    "course_id": 254,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-09T13:24:28.948Z",
    "course_published": true,
    "updated_at": "2016-11-09T13:24:28.931Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":254,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 677e390f79938582d90c29633a7d598ae98eaf1db72247777e6604c9be7b92d7"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/46/bookmarks
Content-Type: application/json
Authorization: Bearer 3297509109ee395ada1e204674222e2fb99f9e274c8d2133ddcb12ac81d97df3
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
    "id": 3,
    "bookmarkable_id": 46,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/46/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3297509109ee395ada1e204674222e2fb99f9e274c8d2133ddcb12ac81d97df3"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/1/votes
Content-Type: application/json
Authorization: Bearer 3142ede565659523d966880a0f9247c9f8237f448ac4a96db8aea227a4d86c3f
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
    "votable_id": 1,
    "user_id": 81
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3142ede565659523d966880a0f9247c9f8237f448ac4a96db8aea227a4d86c3f"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/101/bookmarks
Content-Type: application/json
Authorization: Bearer a05b77b22598be8d55088ca7a018431fc54ddf2d98cfe56e41eaf2d3246ffbf3
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
    "bookmarkable_id": 101,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/101/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a05b77b22598be8d55088ca7a018431fc54ddf2d98cfe56e41eaf2d3246ffbf3"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/122/votes
Content-Type: application/json
Authorization: Bearer 378181f8627b385a13d010b6ad1b1dd890cc7201909f976678240daee53e5223
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 122,
    "user_id": 844
  }
}
```



```shell
curl "api.goskive.com/v2/questions/122/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 378181f8627b385a13d010b6ad1b1dd890cc7201909f976678240daee53e5223"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/23
Content-Type: application/json
Authorization: Bearer a936bfb3d309a5295692fc148dc1ebcbfc1222fbae4f40906f31f35543b3d6e7
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
    "votable_id": 131,
    "user_id": 974
  }
}
```



```shell
curl "api.goskive.com/v2/votes/23" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a936bfb3d309a5295692fc148dc1ebcbfc1222fbae4f40906f31f35543b3d6e7"
```
