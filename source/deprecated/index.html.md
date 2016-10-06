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
Authorization: Bearer 93171166604f5ba73723225059e9dad0bf2fc427f7a81fd77382098603fb7f3a
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
	-H "Authorization: Bearer 93171166604f5ba73723225059e9dad0bf2fc427f7a81fd77382098603fb7f3a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 906132ac7b6bbef7ac5767f926e78d3ea17cff24ce977936da3a423ca7382134
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":97,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":97,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 906132ac7b6bbef7ac5767f926e78d3ea17cff24ce977936da3a423ca7382134"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer acdc02375f7ef6b9188bac4a620a4f76358efd3a22979d31f34754405e3c2ff2
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
201 Created
```


```json
{
  "user_course": {
    "id": 1,
    "course_id": 98,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-06T12:56:59.437Z",
    "course_published": true,
    "updated_at": "2016-10-06T12:56:59.428Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":98,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer acdc02375f7ef6b9188bac4a620a4f76358efd3a22979d31f34754405e3c2ff2"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/47/bookmarks
Content-Type: application/json
Authorization: Bearer 8f7f9234dcd2028339697a75b40f1c6ea121069947bfeb220ea4781a2a8441d6
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
    "id": 4,
    "bookmarkable_id": 47,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/47/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f7f9234dcd2028339697a75b40f1c6ea121069947bfeb220ea4781a2a8441d6"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/14/votes
Content-Type: application/json
Authorization: Bearer befeae0c65dd4349a1df7ac3e0b3a871938fa28b44dfb456b5a83b3b46a2a444
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 14,
    "user_id": 408
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/14/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer befeae0c65dd4349a1df7ac3e0b3a871938fa28b44dfb456b5a83b3b46a2a444"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/11/bookmarks
Content-Type: application/json
Authorization: Bearer 033c3a62a365bfe3208ee8d9d3e9e5cf00e00d7c3caacfb6b6bda73a6f9a0d12
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
    "id": 1,
    "bookmarkable_id": 11,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/11/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 033c3a62a365bfe3208ee8d9d3e9e5cf00e00d7c3caacfb6b6bda73a6f9a0d12"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/106/votes
Content-Type: application/json
Authorization: Bearer 752e19bf776df32e4effaa7e365deff246afa45fa9dc5d64abab1430c58d8b43
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
    "votable_id": 106,
    "user_id": 720
  }
}
```



```shell
curl "api.goskive.com/v2/questions/106/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 752e19bf776df32e4effaa7e365deff246afa45fa9dc5d64abab1430c58d8b43"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/11
Content-Type: application/json
Authorization: Bearer 660d9092bf10a443c9341c610c114525917982b782d51f0cfa326bb102600d2e
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 75,
    "user_id": 533
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 660d9092bf10a443c9341c610c114525917982b782d51f0cfa326bb102600d2e"
```
