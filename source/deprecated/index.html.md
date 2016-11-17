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
DELETE /v2/bookmarks/5
Content-Type: application/json
Authorization: Bearer 591d77b61bc9aaa67e2313d37168bab4bdea5915179035a6e54dce0984f6aa68
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 591d77b61bc9aaa67e2313d37168bab4bdea5915179035a6e54dce0984f6aa68"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 87ae5554d3c22dc9f9f549cb6e75d01641e93a88235b05672cb60ad51604de0c
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":33,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":33,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87ae5554d3c22dc9f9f549cb6e75d01641e93a88235b05672cb60ad51604de0c"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 56d302aba57d338dcbb55977ef7d54cd328aba72be561757fc25f633256bbde3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":32,"pinned":true}}
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
    "course_id": 32,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-17T13:25:39.647Z",
    "course_published": true,
    "updated_at": "2016-11-17T13:25:39.640Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":32,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56d302aba57d338dcbb55977ef7d54cd328aba72be561757fc25f633256bbde3"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/18/bookmarks
Content-Type: application/json
Authorization: Bearer 59eade8391d36c132a738105c39c5e4a491417e9e9490f1d78f6ab3db76fdead
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
    "id": 6,
    "bookmarkable_id": 18,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/18/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59eade8391d36c132a738105c39c5e4a491417e9e9490f1d78f6ab3db76fdead"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/21/votes
Content-Type: application/json
Authorization: Bearer 37ef7c42aca885f4ee6763951b0cc1dc3d414e0d7aebd73a225a2112a148b557
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 21,
    "user_id": 383
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/21/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37ef7c42aca885f4ee6763951b0cc1dc3d414e0d7aebd73a225a2112a148b557"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/71/bookmarks
Content-Type: application/json
Authorization: Bearer 8dc48a0de552a371990176f57f412c8b7f157f4b54dd6c5a32be2d1ff59961b1
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
    "bookmarkable_id": 71,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/71/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8dc48a0de552a371990176f57f412c8b7f157f4b54dd6c5a32be2d1ff59961b1"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/53/votes
Content-Type: application/json
Authorization: Bearer 108b6c3eda2e6473fb3221f59a4f8f92763cb8690712f8af7570adb1c904a92f
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
    "votable_id": 53,
    "user_id": 320
  }
}
```



```shell
curl "api.goskive.com/v2/questions/53/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 108b6c3eda2e6473fb3221f59a4f8f92763cb8690712f8af7570adb1c904a92f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/13
Content-Type: application/json
Authorization: Bearer a3b5b44c3b76ca4730734315c6bbf8168fa3ca5c68c184a918ebdbc107f12c58
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
    "votable_id": 65,
    "user_id": 390
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3b5b44c3b76ca4730734315c6bbf8168fa3ca5c68c184a918ebdbc107f12c58"
```
