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
Authorization: Bearer 4c81039296788df17302ca1669085903801ced70d1d3cd2878f11908acfa81e1
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
	-H "Authorization: Bearer 4c81039296788df17302ca1669085903801ced70d1d3cd2878f11908acfa81e1"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer cafaf02fba3ef7b6d1a50e694d1bddeb3c772fcd069585a0905cbde92a6848d8
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":98,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":98,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cafaf02fba3ef7b6d1a50e694d1bddeb3c772fcd069585a0905cbde92a6848d8"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c13ed26f2317fc13d3b9ed44bccf30966a896c23b7174007c1eda6809d06cdb2
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":99,"pinned":true}}
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
    "course_id": 99,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T14:56:23.196Z",
    "course_published": true,
    "updated_at": "2016-10-27T14:56:23.188Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":99,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c13ed26f2317fc13d3b9ed44bccf30966a896c23b7174007c1eda6809d06cdb2"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/22/bookmarks
Content-Type: application/json
Authorization: Bearer 4e3495f6b4b86d37fcfc25b1741344fb006b4f5a4a23ec4ec1d56dbea0440d5a
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
    "bookmarkable_id": 22,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/22/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e3495f6b4b86d37fcfc25b1741344fb006b4f5a4a23ec4ec1d56dbea0440d5a"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/89/votes
Content-Type: application/json
Authorization: Bearer 31e16f12be51b95fd35e37894fe064d64e41db6eba1486494ca4bcffa61a3ac0
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
    "votable_id": 89,
    "user_id": 920
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/89/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31e16f12be51b95fd35e37894fe064d64e41db6eba1486494ca4bcffa61a3ac0"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/91/bookmarks
Content-Type: application/json
Authorization: Bearer 4cebb51436f028b0d420452c5f88dd5137d40ef62fd6843c22bc62d2041815ef
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
    "bookmarkable_id": 91,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cebb51436f028b0d420452c5f88dd5137d40ef62fd6843c22bc62d2041815ef"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/134/votes
Content-Type: application/json
Authorization: Bearer e6b1a06f40bda912429d5595f8e370124b44ad87ca3df3fa3f4bbe1093392f29
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
    "votable_id": 134,
    "user_id": 976
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6b1a06f40bda912429d5595f8e370124b44ad87ca3df3fa3f4bbe1093392f29"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/2
Content-Type: application/json
Authorization: Bearer 4abd1aae38c417fcd39aa3e2e9e05b2ffa08d4f8a1dd7e07cc7acb269c11e8f4
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
    "id": 2,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 1,
    "user_id": 139
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4abd1aae38c417fcd39aa3e2e9e05b2ffa08d4f8a1dd7e07cc7acb269c11e8f4"
```
