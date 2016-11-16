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
DELETE /v2/bookmarks/9
Content-Type: application/json
Authorization: Bearer b7ff128dfa890e0d61afa430796b22c6c0584a62fd2f077f7ff1230eedefcde3
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7ff128dfa890e0d61afa430796b22c6c0584a62fd2f077f7ff1230eedefcde3"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer fc3163556ac49c2cc3ae8bdb412eab637cc9866ca0984d0fe0a341e5c27d7b5d
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":99,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc3163556ac49c2cc3ae8bdb412eab637cc9866ca0984d0fe0a341e5c27d7b5d"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 10394e071ff0626864856ff3f61f6da6b71df0bb988b2508b1f35489fd615b70
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":100,"pinned":true}}
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
    "course_id": 100,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-16T17:40:58.610Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:40:58.602Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":100,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10394e071ff0626864856ff3f61f6da6b71df0bb988b2508b1f35489fd615b70"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/26/bookmarks
Content-Type: application/json
Authorization: Bearer 95b5fba019adb3182782c4d42b2fcd320551d0a9cb405e3075b84b41374ccab2
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
    "bookmarkable_id": 26,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/26/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95b5fba019adb3182782c4d42b2fcd320551d0a9cb405e3075b84b41374ccab2"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/65/votes
Content-Type: application/json
Authorization: Bearer 2b0e828034c58e3b4abaaf428ff2ad43aba1bc830631672a1e5e4a56e64494dc
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 65,
    "user_id": 752
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/65/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b0e828034c58e3b4abaaf428ff2ad43aba1bc830631672a1e5e4a56e64494dc"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/108/bookmarks
Content-Type: application/json
Authorization: Bearer dc202b48eec1605ace21b5b6d8ded30bc4158319f6831ab19f44e61b9d97b927
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
    "bookmarkable_id": 108,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/108/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc202b48eec1605ace21b5b6d8ded30bc4158319f6831ab19f44e61b9d97b927"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/75/votes
Content-Type: application/json
Authorization: Bearer fc1152838a745cb30f07b0068a2e859a5ef41bdced79d3f6ab6ad3ce902ff438
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 75,
    "user_id": 461
  }
}
```



```shell
curl "api.goskive.com/v2/questions/75/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc1152838a745cb30f07b0068a2e859a5ef41bdced79d3f6ab6ad3ce902ff438"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/13
Content-Type: application/json
Authorization: Bearer bcc636cc34510c2bdfd66f82730fe7bcae12c62cfc02962883e3bb4ccf8b262d
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 111,
    "user_id": 805
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcc636cc34510c2bdfd66f82730fe7bcae12c62cfc02962883e3bb4ccf8b262d"
```
