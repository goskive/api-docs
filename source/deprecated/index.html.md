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
Authorization: Bearer ee9560c0929ebf50296f12ae649f431366339f96580a9fc2a0a69a809cb93ca3
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
	-H "Authorization: Bearer ee9560c0929ebf50296f12ae649f431366339f96580a9fc2a0a69a809cb93ca3"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 252313e984008471ae55859a203e5352551662b196af43b33c0b4b09fbe5f049
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":59,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":59,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 252313e984008471ae55859a203e5352551662b196af43b33c0b4b09fbe5f049"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3e5d069a48af90f3865fab9f200274bfcb947860a45c0778ac6a3d17266a0d29
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":58,"pinned":true}}
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
    "id": 5,
    "course_id": 58,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-09T11:18:15.327Z",
    "course_published": true,
    "updated_at": "2016-11-09T11:18:15.319Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":58,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e5d069a48af90f3865fab9f200274bfcb947860a45c0778ac6a3d17266a0d29"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/42/bookmarks
Content-Type: application/json
Authorization: Bearer c11818f155094de9ccb73c3064c8d81a44eddcdc5d51c9d1ae76237358a24220
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
    "id": 9,
    "bookmarkable_id": 42,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/42/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c11818f155094de9ccb73c3064c8d81a44eddcdc5d51c9d1ae76237358a24220"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/54/votes
Content-Type: application/json
Authorization: Bearer 9f43d611d974bf4273d081144c9acc6494b0f1aa74348ad39c709c7bd23bc2cb
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 54,
    "user_id": 623
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/54/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f43d611d974bf4273d081144c9acc6494b0f1aa74348ad39c709c7bd23bc2cb"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/26/bookmarks
Content-Type: application/json
Authorization: Bearer 3a4e9dcd8f0896f1f3ed661868e9211b3617367708cbea9ebeca864f0bb34404
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
    "bookmarkable_id": 26,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/26/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a4e9dcd8f0896f1f3ed661868e9211b3617367708cbea9ebeca864f0bb34404"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/82/votes
Content-Type: application/json
Authorization: Bearer fff342c9ee7e079ce1b80335ffdfe69d5f36b71e360240b5d6434b0e3d1dd936
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
    "votable_id": 82,
    "user_id": 644
  }
}
```



```shell
curl "api.goskive.com/v2/questions/82/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fff342c9ee7e079ce1b80335ffdfe69d5f36b71e360240b5d6434b0e3d1dd936"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer 04e1c1d067a89d790be4ff1da08ac62e5e8a3f0c3c9d07c43875e5877634b539
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 63,
    "user_id": 490
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04e1c1d067a89d790be4ff1da08ac62e5e8a3f0c3c9d07c43875e5877634b539"
```
