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
Authorization: Bearer c2b24ef0e0d6e62d72e75ab46ca0bfbdc77102e9f0dd9276e6598232d1342e8a
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
	-H "Authorization: Bearer c2b24ef0e0d6e62d72e75ab46ca0bfbdc77102e9f0dd9276e6598232d1342e8a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 773b4a09a15348db20ac8a1b347724ceb7ab1026b311bfa840bf0cd5564e2f05
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":186,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":186,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 773b4a09a15348db20ac8a1b347724ceb7ab1026b311bfa840bf0cd5564e2f05"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 98657157b8dd55c8b1a6d2724a58008db5778a40805b86af3a773bf7a5685446
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
201 Created
```


```json
{
  "user_course": {
    "id": 6,
    "course_id": 185,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T17:13:11.162Z",
    "course_published": true,
    "updated_at": "2016-10-25T17:13:11.155Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":185,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98657157b8dd55c8b1a6d2724a58008db5778a40805b86af3a773bf7a5685446"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/13/bookmarks
Content-Type: application/json
Authorization: Bearer f9357c6307af800368434214905f0dec0c0f983e3194e88af184f6a53ebb7980
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
    "bookmarkable_id": 13,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/13/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9357c6307af800368434214905f0dec0c0f983e3194e88af184f6a53ebb7980"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/53/votes
Content-Type: application/json
Authorization: Bearer c5a1574bc6ed4a97ca1794c6f8a9472e7012d2e0f1d2d6203e3b0da5670fd2c5
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
    "votable_id": 53,
    "user_id": 522
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5a1574bc6ed4a97ca1794c6f8a9472e7012d2e0f1d2d6203e3b0da5670fd2c5"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/98/bookmarks
Content-Type: application/json
Authorization: Bearer ccb372fea886db636a14890ebafd92291a4dfdb821919b761140ad6b11264a94
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
    "bookmarkable_id": 98,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/98/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccb372fea886db636a14890ebafd92291a4dfdb821919b761140ad6b11264a94"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/108/votes
Content-Type: application/json
Authorization: Bearer d85b1d30a3932c76d306f85b431503698ddb8dd8440a2e6ef1737558162ba3fc
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
    "votable_id": 108,
    "user_id": 859
  }
}
```



```shell
curl "api.goskive.com/v2/questions/108/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d85b1d30a3932c76d306f85b431503698ddb8dd8440a2e6ef1737558162ba3fc"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/17
Content-Type: application/json
Authorization: Bearer 296d8158c755f3e55dbaf10b561772b150448d1298b8499f60b7dabadfb9d667
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
    "votable_id": 100,
    "user_id": 785
  }
}
```



```shell
curl "api.goskive.com/v2/votes/17" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 296d8158c755f3e55dbaf10b561772b150448d1298b8499f60b7dabadfb9d667"
```
