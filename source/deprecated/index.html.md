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
DELETE /v2/bookmarks/8
Content-Type: application/json
Authorization: Bearer 7caa59fbe43ef6f52ea9aafd0f4cad57d4cc9f37443e970b8551045d34f91450
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7caa59fbe43ef6f52ea9aafd0f4cad57d4cc9f37443e970b8551045d34f91450"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 59bc4ee446cbb510fd0a260cd8bac9b04cd5d0fcdb8a95949d9a8f6ef46041d3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":133,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":133,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59bc4ee446cbb510fd0a260cd8bac9b04cd5d0fcdb8a95949d9a8f6ef46041d3"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 324594e1f175ae571c579c7d6659759361ad4797abed098084a525b001143303
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":132,"pinned":true}}
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
    "course_id": 132,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-26T08:42:27.188Z",
    "course_published": true,
    "updated_at": "2016-09-26T08:42:27.178Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":132,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 324594e1f175ae571c579c7d6659759361ad4797abed098084a525b001143303"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/12/bookmarks
Content-Type: application/json
Authorization: Bearer 55de42f4df2017a9cb7297645d566d36a5c4f08140587306e881c5d5ce109bb8
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
    "bookmarkable_id": 12,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/12/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55de42f4df2017a9cb7297645d566d36a5c4f08140587306e881c5d5ce109bb8"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/3/votes
Content-Type: application/json
Authorization: Bearer 92bc66d6a653dd6a2b5c583b3eaebf6410d2e79bf0faac8d289ef217d2415742
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 3,
    "user_id": 10
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92bc66d6a653dd6a2b5c583b3eaebf6410d2e79bf0faac8d289ef217d2415742"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/44/bookmarks
Content-Type: application/json
Authorization: Bearer 5fe4126000f7d28a314dbde12932dfab3ba31a66ebb1802a17e8662cff759112
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
    "bookmarkable_id": 44,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/44/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fe4126000f7d28a314dbde12932dfab3ba31a66ebb1802a17e8662cff759112"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/96/votes
Content-Type: application/json
Authorization: Bearer 1fc60b500656fbceb011b288e1aca9770fe1938c2c92305a3523f12ddc0e20a4
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
    "votable_id": 96,
    "user_id": 724
  }
}
```



```shell
curl "api.goskive.com/v2/questions/96/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fc60b500656fbceb011b288e1aca9770fe1938c2c92305a3523f12ddc0e20a4"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/9
Content-Type: application/json
Authorization: Bearer b9c79516f2879ff44af72bbc6c361a3659f774069e06c5c188010bac9380970a
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 54,
    "user_id": 296
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9c79516f2879ff44af72bbc6c361a3659f774069e06c5c188010bac9380970a"
```
