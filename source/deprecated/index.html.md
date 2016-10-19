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
Authorization: Bearer c8c762bc0b2668b1ea6696907b00be0e285c71e8c5aa3ebcf40e60aaa77cb50d
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
	-H "Authorization: Bearer c8c762bc0b2668b1ea6696907b00be0e285c71e8c5aa3ebcf40e60aaa77cb50d"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8fb3bd8ac3a0635c9e52a8689f75535548f2fc9c8f723eb6ec3c59bc5430e3a9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":162,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":162,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fb3bd8ac3a0635c9e52a8689f75535548f2fc9c8f723eb6ec3c59bc5430e3a9"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 871c99f4904692713beb48f305db578b43646b83b488925c56044d975594cc35
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":161,"pinned":true}}
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
    "course_id": 161,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T09:00:10.061Z",
    "course_published": true,
    "updated_at": "2016-10-19T09:00:10.053Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":161,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 871c99f4904692713beb48f305db578b43646b83b488925c56044d975594cc35"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/9/bookmarks
Content-Type: application/json
Authorization: Bearer da7d0b6b0d33d715ee250ba2f5480d8f6ab500e5d9eb69375c0ecb3ab5c5fee6
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
    "bookmarkable_id": 9,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/9/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da7d0b6b0d33d715ee250ba2f5480d8f6ab500e5d9eb69375c0ecb3ab5c5fee6"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/90/votes
Content-Type: application/json
Authorization: Bearer df829d1a98d447f99241b04cd2ce073865072df1200cbb8a86d05a332d898e9b
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 90,
    "user_id": 868
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/90/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df829d1a98d447f99241b04cd2ce073865072df1200cbb8a86d05a332d898e9b"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/132/bookmarks
Content-Type: application/json
Authorization: Bearer 60ae8888e33b92c7fdd6de94f0b1a38dd8a6e625ff689bbc76597878141262e5
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
    "bookmarkable_id": 132,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/132/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60ae8888e33b92c7fdd6de94f0b1a38dd8a6e625ff689bbc76597878141262e5"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/131/votes
Content-Type: application/json
Authorization: Bearer 45e107353fb7ab5e1706e601154dda12d809b0bb9833f6eacb3e6f5c26dfbc10
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
    "id": 22,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 131,
    "user_id": 944
  }
}
```



```shell
curl "api.goskive.com/v2/questions/131/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45e107353fb7ab5e1706e601154dda12d809b0bb9833f6eacb3e6f5c26dfbc10"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/4
Content-Type: application/json
Authorization: Bearer bf0dd8bd717ac32ff61f528953100ce8e96584d527a4fb6891c8bbb9e202bfec
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 87,
    "user_id": 448
  }
}
```



```shell
curl "api.goskive.com/v2/votes/4" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf0dd8bd717ac32ff61f528953100ce8e96584d527a4fb6891c8bbb9e202bfec"
```
