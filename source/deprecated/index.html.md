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
DELETE /v2/bookmarks/2
Content-Type: application/json
Authorization: Bearer 4a748abc6c91ec935bb60988cfc5f5954223cf8a08a8d80542f42f57bed8e499
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a748abc6c91ec935bb60988cfc5f5954223cf8a08a8d80542f42f57bed8e499"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 71ef544d2a94c7c227b3625382767850b419f5cb982182c2a58f4ebe4d549cef
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":187,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":187,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71ef544d2a94c7c227b3625382767850b419f5cb982182c2a58f4ebe4d549cef"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 03f1d3a8086e214e768b22eee7a317ac7ca8a6838a222b69ceeb0df12c26962d
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":188,"pinned":true}}
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
    "course_id": 188,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T14:21:43.531Z",
    "course_published": true,
    "updated_at": "2016-11-08T14:21:43.522Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":188,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03f1d3a8086e214e768b22eee7a317ac7ca8a6838a222b69ceeb0df12c26962d"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/1/bookmarks
Content-Type: application/json
Authorization: Bearer 52f2f40a42b7b056cb3748eaff26ca20a4d991b2288c662ac95701003f090b5d
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
    "bookmarkable_id": 1,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52f2f40a42b7b056cb3748eaff26ca20a4d991b2288c662ac95701003f090b5d"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/48/votes
Content-Type: application/json
Authorization: Bearer 03f474032669bd3d1c5c07588a2d206a660bd2e087948f6067e6fd7b5d137f0e
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
    "votable_id": 48,
    "user_id": 332
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/48/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03f474032669bd3d1c5c07588a2d206a660bd2e087948f6067e6fd7b5d137f0e"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/95/bookmarks
Content-Type: application/json
Authorization: Bearer 9f05248f9f3533e4202223f659c7298f1f737714628dfda0ae4e1629a576f7b1
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
    "bookmarkable_id": 95,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f05248f9f3533e4202223f659c7298f1f737714628dfda0ae4e1629a576f7b1"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/102/votes
Content-Type: application/json
Authorization: Bearer 9505dbf4e8b8fc7f9355d99df4a5681284014e72fefccc464db4809ed66abf8c
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 102,
    "user_id": 822
  }
}
```



```shell
curl "api.goskive.com/v2/questions/102/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9505dbf4e8b8fc7f9355d99df4a5681284014e72fefccc464db4809ed66abf8c"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/2
Content-Type: application/json
Authorization: Bearer 1a5c082c079081e19f3e85dbba86adf7db45e821ce5fdc09afc5feef966dc9c4
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
    "votable_id": 16,
    "user_id": 214
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a5c082c079081e19f3e85dbba86adf7db45e821ce5fdc09afc5feef966dc9c4"
```
