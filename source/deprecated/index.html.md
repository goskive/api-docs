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
Authorization: Bearer ed274e8dc05573dd664a2f652833b6533b8daa3c4e279a465efaf0d11959ff3e
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
	-H "Authorization: Bearer ed274e8dc05573dd664a2f652833b6533b8daa3c4e279a465efaf0d11959ff3e"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer d084090b121b0a2541f7c36b521c7d961e8b22835b480832392cbf536bd84a18
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":242,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":242,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d084090b121b0a2541f7c36b521c7d961e8b22835b480832392cbf536bd84a18"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a943ac78cf6e3e41d189b7bfe4cc6cedbcd151af31acac0b37b526a9f63f5b2c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":241,"pinned":true}}
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
    "id": 12,
    "course_id": 241,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-08T12:16:47.524Z",
    "course_published": true,
    "updated_at": "2016-09-08T12:16:47.515Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":241,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a943ac78cf6e3e41d189b7bfe4cc6cedbcd151af31acac0b37b526a9f63f5b2c"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/89/bookmarks
Content-Type: application/json
Authorization: Bearer a1b4e8f9bccf04b6ba9c140b9e03c29e42fc283ac174f8071a20c82b95a667e5
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
    "bookmarkable_id": 89,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/89/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1b4e8f9bccf04b6ba9c140b9e03c29e42fc283ac174f8071a20c82b95a667e5"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/66/votes
Content-Type: application/json
Authorization: Bearer 3536dd2a86f71e4958b4d9f40fda011bb83c4e791a685c2e578e85b2b6f0361c
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 66,
    "user_id": 406
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/66/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3536dd2a86f71e4958b4d9f40fda011bb83c4e791a685c2e578e85b2b6f0361c"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/1/bookmarks
Content-Type: application/json
Authorization: Bearer 955e47c72700507490f74495c8134f73bd7e304f5b8c804695cc7f44c935e222
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
    "bookmarkable_id": 1,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 955e47c72700507490f74495c8134f73bd7e304f5b8c804695cc7f44c935e222"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/93/votes
Content-Type: application/json
Authorization: Bearer 418c67531b069ddfd3e54152cbd7056e5b4ef01d92302688149e776571a6ba5a
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
    "votable_id": 93,
    "user_id": 576
  }
}
```



```shell
curl "api.goskive.com/v2/questions/93/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 418c67531b069ddfd3e54152cbd7056e5b4ef01d92302688149e776571a6ba5a"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/18
Content-Type: application/json
Authorization: Bearer 65d148b14fe2a9bf12b3ca3ae676c4802427bf960f56c2795fc3db445f05e509
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 94,
    "user_id": 579
  }
}
```



```shell
curl "api.goskive.com/v2/votes/18" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65d148b14fe2a9bf12b3ca3ae676c4802427bf960f56c2795fc3db445f05e509"
```
