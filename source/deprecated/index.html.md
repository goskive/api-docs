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
DELETE /v2/bookmarks/1
Content-Type: application/json
Authorization: Bearer b9ca06753ad2775fa26a19f0e4d6effbea205755a7465cd80aa7a1ee36c7e82e
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
	-H "Authorization: Bearer b9ca06753ad2775fa26a19f0e4d6effbea205755a7465cd80aa7a1ee36c7e82e"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 708a1cdb534320064e06a34f3d817ce795ba4e94003ec0feb723ef1beef6edd1
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":9,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":9,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 708a1cdb534320064e06a34f3d817ce795ba4e94003ec0feb723ef1beef6edd1"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b73bbafcf68d3dfb7fbca415fe344b789d24ef8f3112fae00742fe3bdf9ab588
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":10,"pinned":true}}
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
    "id": 2,
    "course_id": 10,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T12:01:25.322Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:01:25.313Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":10,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b73bbafcf68d3dfb7fbca415fe344b789d24ef8f3112fae00742fe3bdf9ab588"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/43/bookmarks
Content-Type: application/json
Authorization: Bearer 4b1f61bd6b502de8dacaf4c81ec1e1511b95156243781f67a8a8fcae0cee902d
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
    "id": 3,
    "bookmarkable_id": 43,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b1f61bd6b502de8dacaf4c81ec1e1511b95156243781f67a8a8fcae0cee902d"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/12/votes
Content-Type: application/json
Authorization: Bearer 43db152a7b6d8dee677eddf825cee24fc2fb7486cef0750dbc0fd4cb3bf3c696
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 12,
    "user_id": 124
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/12/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43db152a7b6d8dee677eddf825cee24fc2fb7486cef0750dbc0fd4cb3bf3c696"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/18/bookmarks
Content-Type: application/json
Authorization: Bearer e7730e9ad7d9afebf8bddd377129c6e1138fa8a8945b0264b9b3eca63d61c94c
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
    "bookmarkable_id": 18,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/18/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7730e9ad7d9afebf8bddd377129c6e1138fa8a8945b0264b9b3eca63d61c94c"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/6/votes
Content-Type: application/json
Authorization: Bearer 2bced3fa7a093ff0a95e029612251fcd07e88406df3cf8e1e7b97fc56bb95a82
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 6,
    "user_id": 22
  }
}
```



```shell
curl "api.goskive.com/v2/questions/6/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bced3fa7a093ff0a95e029612251fcd07e88406df3cf8e1e7b97fc56bb95a82"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/2
Content-Type: application/json
Authorization: Bearer f419040da50c6ecf9c006f1c6a234b9b46446b1af002eef8c2b2bd275d01570f
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
    "user_id": 5
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f419040da50c6ecf9c006f1c6a234b9b46446b1af002eef8c2b2bd275d01570f"
```
