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
Authorization: Bearer d97d934e0da6f10e4952992a029bbc7a7c1a6ed24482c9f762736a5d070b1bde
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
	-H "Authorization: Bearer d97d934e0da6f10e4952992a029bbc7a7c1a6ed24482c9f762736a5d070b1bde"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1c61eabe82578713ab5b677dfa58d8be4016a671cc0e16d4c7e901bb2935774f
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":185,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":185,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c61eabe82578713ab5b677dfa58d8be4016a671cc0e16d4c7e901bb2935774f"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 42b4700185474a4aedf7f23b7bb1ddce0cf058b4a0169d2be0b3221bbcb3b8ed
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":184,"pinned":true}}
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
    "course_id": 184,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T10:12:00.934Z",
    "course_published": true,
    "updated_at": "2016-10-26T10:12:00.926Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":184,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42b4700185474a4aedf7f23b7bb1ddce0cf058b4a0169d2be0b3221bbcb3b8ed"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/30/bookmarks
Content-Type: application/json
Authorization: Bearer 2fda2945df03beaef4ddb7ad84aad0c6dd844d4ee03fc38d00589c6e25d6d71e
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
    "bookmarkable_id": 30,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/30/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2fda2945df03beaef4ddb7ad84aad0c6dd844d4ee03fc38d00589c6e25d6d71e"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/33/votes
Content-Type: application/json
Authorization: Bearer 122f68117c5e8795bf51905cc9bbac69fb261fd34ec5a126b68572111712f5e5
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
    "votable_id": 33,
    "user_id": 572
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 122f68117c5e8795bf51905cc9bbac69fb261fd34ec5a126b68572111712f5e5"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/86/bookmarks
Content-Type: application/json
Authorization: Bearer 9f2ae60846660320b81acff994f7b9e850f8c13deb983190bf6f952189aea63b
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
    "bookmarkable_id": 86,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/86/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f2ae60846660320b81acff994f7b9e850f8c13deb983190bf6f952189aea63b"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/11/votes
Content-Type: application/json
Authorization: Bearer 2567cc9e3f83f3e39914ac8bf1af2e73d7388aadd443194ef5cc4ade8e4bf2ac
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 11,
    "user_id": 73
  }
}
```



```shell
curl "api.goskive.com/v2/questions/11/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2567cc9e3f83f3e39914ac8bf1af2e73d7388aadd443194ef5cc4ade8e4bf2ac"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/17
Content-Type: application/json
Authorization: Bearer dc2e7232e166c090042b758399017917c920636dcb9006eaea47c724216433b7
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
    "id": 17,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 123,
    "user_id": 871
  }
}
```



```shell
curl "api.goskive.com/v2/votes/17" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc2e7232e166c090042b758399017917c920636dcb9006eaea47c724216433b7"
```
