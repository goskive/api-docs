---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Bookmarks

## Delete a bookmark

DEPRECATED. Use DELETE /v2/:content_unit_type/:content_unit_id/bookmark instead.

### Request

#### Endpoint

```
DELETE /v2/bookmarks/1
Content-Type: application/json
Authorization: Bearer b3eb77454ed18a3371a062bdd40eee95cef6a490a15b417877c6bdb0ff6f0aac
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3eb77454ed18a3371a062bdd40eee95cef6a490a15b417877c6bdb0ff6f0aac"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 269f160a9485ec90257fd5df1e0c11289a7c468d947fe3e134edbfbd725e6b97
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":150,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":150,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 269f160a9485ec90257fd5df1e0c11289a7c468d947fe3e134edbfbd725e6b97"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a986eb3b328f82db2bddd4dbae483e780097a7cc6628e030c56fd84d4c7cfcc6
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":151,"pinned":true}}
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
    "id": 7,
    "course_id": 151,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T17:20:10.343Z",
    "course_published": true,
    "updated_at": "2016-12-15T17:20:10.337Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":151,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a986eb3b328f82db2bddd4dbae483e780097a7cc6628e030c56fd84d4c7cfcc6"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/56/bookmarks
Content-Type: application/json
Authorization: Bearer 5df75c32a85910a5d3dcb6b6f733faf906c2f90a10ad9e1e1a730e2d565bee06
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
    "bookmarkable_id": 56,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5df75c32a85910a5d3dcb6b6f733faf906c2f90a10ad9e1e1a730e2d565bee06"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/37/votes
Content-Type: application/json
Authorization: Bearer 8f919ed3031c070013cef3e215e15ef8e02e95220f5766ecf8d4c1a3bdfaf4e7
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 37,
    "user_id": 256
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/37/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f919ed3031c070013cef3e215e15ef8e02e95220f5766ecf8d4c1a3bdfaf4e7"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/23/bookmarks
Content-Type: application/json
Authorization: Bearer e60cc5e248758079fe33622632f4fd4742e544c6fe52cceb35bd502d2d152bc3
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
    "id": 3,
    "bookmarkable_id": 23,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/23/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e60cc5e248758079fe33622632f4fd4742e544c6fe52cceb35bd502d2d152bc3"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer 7b3db37788f39a136f754ebb98e9c6922f565dc9aee37874a697f74115f0a078
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 10
  }
}
```



```shell
curl "api.goskive.com/v2/questions/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b3db37788f39a136f754ebb98e9c6922f565dc9aee37874a697f74115f0a078"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/19
Content-Type: application/json
Authorization: Bearer ac628b6df01e8f7fd8ae7135b9ead598d7b208b66cfc817746b890efba0365fb
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
    "votable_id": 126,
    "user_id": 850
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac628b6df01e8f7fd8ae7135b9ead598d7b208b66cfc817746b890efba0365fb"
```
