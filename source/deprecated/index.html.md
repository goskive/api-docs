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
DELETE /v2/bookmarks/4
Content-Type: application/json
Authorization: Bearer 60ae6c6bcd63086ca530f4d7ca00b53231914fb057b1b0ca981adae0bacd5c6b
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60ae6c6bcd63086ca530f4d7ca00b53231914fb057b1b0ca981adae0bacd5c6b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer e3a1f131510125bcc75f07447f640a860302929b0fc2f5d281f4d4a0d57e3274
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":157,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":157,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3a1f131510125bcc75f07447f640a860302929b0fc2f5d281f4d4a0d57e3274"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 56ad0e36b7090c3c57f70810d1b8eb6618039be414556e142ba211c144977d05
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":156,"pinned":true}}
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
    "course_id": 156,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T10:35:32.065Z",
    "course_published": true,
    "updated_at": "2016-10-26T10:35:32.056Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":156,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56ad0e36b7090c3c57f70810d1b8eb6618039be414556e142ba211c144977d05"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/40/bookmarks
Content-Type: application/json
Authorization: Bearer b49b0b96a42e33a25aabc774d4b6bcc10d1beb459702d3dbca3ae1b99395b0fc
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
    "bookmarkable_id": 40,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/40/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b49b0b96a42e33a25aabc774d4b6bcc10d1beb459702d3dbca3ae1b99395b0fc"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/7/votes
Content-Type: application/json
Authorization: Bearer a925c0bade6ca2291da6db244ac7cbe3d963c87989bf7f74ea71aa14f20acf39
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 7,
    "user_id": 27
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/7/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a925c0bade6ca2291da6db244ac7cbe3d963c87989bf7f74ea71aa14f20acf39"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/131/bookmarks
Content-Type: application/json
Authorization: Bearer c1b539a4358cbcf1e2d746c823cc8b26291450026ef58801570b4e2d69e23378
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
    "id": 6,
    "bookmarkable_id": 131,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/131/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1b539a4358cbcf1e2d746c823cc8b26291450026ef58801570b4e2d69e23378"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/122/votes
Content-Type: application/json
Authorization: Bearer 0ceed9b66aa2770d4246a52a804f73270757c32b5f059cdb8d5d3f850edced73
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
    "votable_id": 122,
    "user_id": 927
  }
}
```



```shell
curl "api.goskive.com/v2/questions/122/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ceed9b66aa2770d4246a52a804f73270757c32b5f059cdb8d5d3f850edced73"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/18
Content-Type: application/json
Authorization: Bearer af1e94100e964ed33685a47dcb3616cbd54f7ddbf3bdd2d3189376b1b90a454e
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 119,
    "user_id": 883
  }
}
```



```shell
curl "api.goskive.com/v2/votes/18" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af1e94100e964ed33685a47dcb3616cbd54f7ddbf3bdd2d3189376b1b90a454e"
```
