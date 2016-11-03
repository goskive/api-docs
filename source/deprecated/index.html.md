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
Authorization: Bearer a532cfa38ce1b6f5a24cea9fe89f70f6ae2e7dc010f63a7490fc3134d416960a
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
	-H "Authorization: Bearer a532cfa38ce1b6f5a24cea9fe89f70f6ae2e7dc010f63a7490fc3134d416960a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 711644568f4c40bc11d478e316e8a28cd88c6bf956f2c65bfb1baddd818da22b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":275,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":275,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 711644568f4c40bc11d478e316e8a28cd88c6bf956f2c65bfb1baddd818da22b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 85e97507e89386e62dbce4d327e958a7ef3bd6d772a4a1a43d763eacefb51978
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":274,"pinned":true}}
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
    "course_id": 274,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T17:48:49.420Z",
    "course_published": true,
    "updated_at": "2016-11-03T17:48:49.412Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":274,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85e97507e89386e62dbce4d327e958a7ef3bd6d772a4a1a43d763eacefb51978"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/49/bookmarks
Content-Type: application/json
Authorization: Bearer a179f7aa0fba140e0209a5ef1969c75881181a3a3f1d2840a231f0d60216c422
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
    "id": 7,
    "bookmarkable_id": 49,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/49/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a179f7aa0fba140e0209a5ef1969c75881181a3a3f1d2840a231f0d60216c422"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/56/votes
Content-Type: application/json
Authorization: Bearer be3d01ed59fc359e36c72e2b6d01ead8aa74150b7176eae4c984149a725e4eab
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
    "votable_id": 56,
    "user_id": 621
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be3d01ed59fc359e36c72e2b6d01ead8aa74150b7176eae4c984149a725e4eab"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/131/bookmarks
Content-Type: application/json
Authorization: Bearer 9e3723b6614ab97f1f876b20e288449dc03c150db7033bc92b4c1fe0e0cc3981
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
    "id": 10,
    "bookmarkable_id": 131,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/131/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e3723b6614ab97f1f876b20e288449dc03c150db7033bc92b4c1fe0e0cc3981"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/134/votes
Content-Type: application/json
Authorization: Bearer b262dbbb592824ab6f023996e094cef5f32e318e59007c3cd4ca5d922fa823ed
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
    "user_id": 986
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b262dbbb592824ab6f023996e094cef5f32e318e59007c3cd4ca5d922fa823ed"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/3
Content-Type: application/json
Authorization: Bearer 6cca867e9af5539772fdbba354810a951cac852416fb017da089d5c1d2ace17a
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
    "id": 3,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 6,
    "user_id": 81
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cca867e9af5539772fdbba354810a951cac852416fb017da089d5c1d2ace17a"
```
