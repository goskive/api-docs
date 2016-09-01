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
Authorization: Bearer dd4a6e6ac669a983907410599d9970a96ce4a99c6bbe576caf6bd09cd3bf3e62
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
	-H "Authorization: Bearer dd4a6e6ac669a983907410599d9970a96ce4a99c6bbe576caf6bd09cd3bf3e62"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c968e2f1fa38ad0f4e1e92cf548e3828bc9fe6154c8e895c5c32674fa8993da4
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":14,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":14,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c968e2f1fa38ad0f4e1e92cf548e3828bc9fe6154c8e895c5c32674fa8993da4"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f9f0f782a718804c405a42441ad03d5288ccab2b3ac97b9511c249babea85b17
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":15,"pinned":true}}
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
    "course_id": 15,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-01T13:38:18.052Z",
    "course_published": true,
    "updated_at": "2016-09-01T13:38:18.043Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":15,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9f0f782a718804c405a42441ad03d5288ccab2b3ac97b9511c249babea85b17"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/33/bookmarks
Content-Type: application/json
Authorization: Bearer d3aa35a8d03280433f8ca58d5abfc4b6abdbf2e80263a84dfa5adf85bf2fce1c
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
    "id": 5,
    "bookmarkable_id": 33,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3aa35a8d03280433f8ca58d5abfc4b6abdbf2e80263a84dfa5adf85bf2fce1c"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/63/votes
Content-Type: application/json
Authorization: Bearer 029dbeca8eb1948230ab0a52d0def930ebbc0ed861ce60f17ca20b81272d49c8
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 63,
    "user_id": 718
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/63/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 029dbeca8eb1948230ab0a52d0def930ebbc0ed861ce60f17ca20b81272d49c8"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/125/bookmarks
Content-Type: application/json
Authorization: Bearer cfacb05b4c92f7e3573005030848728370f8a2a214c710dcb5d43658aed64054
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
    "bookmarkable_id": 125,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/125/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfacb05b4c92f7e3573005030848728370f8a2a214c710dcb5d43658aed64054"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/124/votes
Content-Type: application/json
Authorization: Bearer c02014b70572fa1752c9a66eed95d60e43046b647d441138caec3420b97f1b90
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
    "votable_id": 124,
    "user_id": 913
  }
}
```



```shell
curl "api.goskive.com/v2/questions/124/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c02014b70572fa1752c9a66eed95d60e43046b647d441138caec3420b97f1b90"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/2
Content-Type: application/json
Authorization: Bearer a9b8ead743205dd704a67f338b93f9ccada6dac2d6215cdd0154b88a95264c4d
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
    "votable_id": 2,
    "user_id": 19
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9b8ead743205dd704a67f338b93f9ccada6dac2d6215cdd0154b88a95264c4d"
```
