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
Authorization: Bearer 0ba6bbbbb9c5ed7fd70884cd90517de0f6f3e90169f9e392c34e8eb953c3bee4
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
	-H "Authorization: Bearer 0ba6bbbbb9c5ed7fd70884cd90517de0f6f3e90169f9e392c34e8eb953c3bee4"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer cf888cd81421989b7e4b5e63fde1a0b86222a523198e12486f35f992d6eddcdb
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":245,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":245,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf888cd81421989b7e4b5e63fde1a0b86222a523198e12486f35f992d6eddcdb"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9edcda5bc80b79413738c7af9503ea140bf81ebd6fa9ab471c95b77221a20cd0
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":246,"pinned":true}}
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
    "course_id": 246,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-17T14:14:41.051Z",
    "course_published": true,
    "updated_at": "2016-11-17T14:14:41.042Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":246,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9edcda5bc80b79413738c7af9503ea140bf81ebd6fa9ab471c95b77221a20cd0"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/9/bookmarks
Content-Type: application/json
Authorization: Bearer 0975ac9bb121e661f9f72f250e6d2b5ffb2725d8cabf6602b9002a6697b241c7
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
    "bookmarkable_id": 9,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/9/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0975ac9bb121e661f9f72f250e6d2b5ffb2725d8cabf6602b9002a6697b241c7"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/1/votes
Content-Type: application/json
Authorization: Bearer f40ceb388f1cec7deb5e520f5f8e54d788d5bf6ec449eaaf1319bef02171cfbc
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
    "id": 2,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 1,
    "user_id": 64
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f40ceb388f1cec7deb5e520f5f8e54d788d5bf6ec449eaaf1319bef02171cfbc"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/91/bookmarks
Content-Type: application/json
Authorization: Bearer 10da0278cbee7a4b8927672947d0ce10426b3425c9b39b8334bd029271582569
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
    "bookmarkable_id": 91,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10da0278cbee7a4b8927672947d0ce10426b3425c9b39b8334bd029271582569"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/107/votes
Content-Type: application/json
Authorization: Bearer 639908ce7d7843387f8c3918f9a067794db6f519169a5f927d44f8e4ce1e16af
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
    "votable_id": 107,
    "user_id": 817
  }
}
```



```shell
curl "api.goskive.com/v2/questions/107/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 639908ce7d7843387f8c3918f9a067794db6f519169a5f927d44f8e4ce1e16af"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/6
Content-Type: application/json
Authorization: Bearer 648cbc8f6d7a9defa8d32dc9c94b1561d73562bef7e444ef502cc5205b1e344f
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
    "votable_id": 3,
    "user_id": 76
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 648cbc8f6d7a9defa8d32dc9c94b1561d73562bef7e444ef502cc5205b1e344f"
```
