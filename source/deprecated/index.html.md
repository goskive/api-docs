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
DELETE /v2/bookmarks/10
Content-Type: application/json
Authorization: Bearer 4ac7f9b4d5805aecfbcf779ed49d0dfa7728134dada93aadb7d62f1b61e9c043
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ac7f9b4d5805aecfbcf779ed49d0dfa7728134dada93aadb7d62f1b61e9c043"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1eb6e2d51c6f0b96eacab6b768bc3078ec91021ab1bef68efaab1ffc43f60d42
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":152,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":152,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1eb6e2d51c6f0b96eacab6b768bc3078ec91021ab1bef68efaab1ffc43f60d42"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer fc8fe260e360314f5cf94ddbf2b03f92c7ffcfb6b549eb6e893cca4504b2ef53
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
    "id": 5,
    "course_id": 151,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-04T16:00:45.896Z",
    "course_published": true,
    "updated_at": "2016-11-04T16:00:45.888Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":151,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc8fe260e360314f5cf94ddbf2b03f92c7ffcfb6b549eb6e893cca4504b2ef53"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/17/bookmarks
Content-Type: application/json
Authorization: Bearer b3d6f1ad0bec80670a70c160dbde2646a431fe4e1dfdfea7659bb3f852e3ee20
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
    "bookmarkable_id": 17,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/17/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3d6f1ad0bec80670a70c160dbde2646a431fe4e1dfdfea7659bb3f852e3ee20"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/48/votes
Content-Type: application/json
Authorization: Bearer 0ef5c826558df13edf6721601a106ebc0b0a8f02de17ff95c123d9eb73d4eb35
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
    "user_id": 396
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/48/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ef5c826558df13edf6721601a106ebc0b0a8f02de17ff95c123d9eb73d4eb35"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/34/bookmarks
Content-Type: application/json
Authorization: Bearer 352cdb18946d5a3d0135169986afaaf22a12bf6b35da00999b5b656dd85cfcb0
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
    "bookmarkable_id": 34,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/34/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 352cdb18946d5a3d0135169986afaaf22a12bf6b35da00999b5b656dd85cfcb0"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/31/votes
Content-Type: application/json
Authorization: Bearer d7f3b0a5cc2ef157fa8d450f53914c7098f65683bc2a966d76b153c72fe68e1b
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 31,
    "user_id": 238
  }
}
```



```shell
curl "api.goskive.com/v2/questions/31/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7f3b0a5cc2ef157fa8d450f53914c7098f65683bc2a966d76b153c72fe68e1b"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/6
Content-Type: application/json
Authorization: Bearer 7dbbb96d851372b71528f11968ab8e3eec2f1fe4b596c97d6b1e487cb326b074
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 62,
    "user_id": 324
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dbbb96d851372b71528f11968ab8e3eec2f1fe4b596c97d6b1e487cb326b074"
```
