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
Authorization: Bearer 001b23d0926ea18c592e4a6913e50d4d37c443669909f1f9514028804f09ab0c
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
	-H "Authorization: Bearer 001b23d0926ea18c592e4a6913e50d4d37c443669909f1f9514028804f09ab0c"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3f58e8dd15a7edff7754b4a09158a4f426d6b900f048f9706d0245d675647f0e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":199,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":199,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f58e8dd15a7edff7754b4a09158a4f426d6b900f048f9706d0245d675647f0e"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b8a57c29c98fd422fb275e3c5c491fa6152847416a89d5610995fd869e33f632
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":200,"pinned":true}}
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
    "id": 4,
    "course_id": 200,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T17:43:44.444Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:43:44.436Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":200,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8a57c29c98fd422fb275e3c5c491fa6152847416a89d5610995fd869e33f632"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/67/bookmarks
Content-Type: application/json
Authorization: Bearer 08b85db1f7f8ad659b6335e7e0e2d9f13e74db2d5a8da1003d124e780538d6ef
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
    "id": 9,
    "bookmarkable_id": 67,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/67/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08b85db1f7f8ad659b6335e7e0e2d9f13e74db2d5a8da1003d124e780538d6ef"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/68/votes
Content-Type: application/json
Authorization: Bearer 1d3c50051761432e46854d4a6ce93f420aa5765576d30c2e20cc37bf3ea6bbbb
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 68,
    "user_id": 656
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/68/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d3c50051761432e46854d4a6ce93f420aa5765576d30c2e20cc37bf3ea6bbbb"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/87/bookmarks
Content-Type: application/json
Authorization: Bearer 588761e10f731d83b54990306176300b703a085948ff77b02eef1827062e1eb5
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
    "bookmarkable_id": 87,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/87/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 588761e10f731d83b54990306176300b703a085948ff77b02eef1827062e1eb5"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/98/votes
Content-Type: application/json
Authorization: Bearer 228d5d634f2837395c7edb1ff68c1f84e9f2ab10784fb98fd24f36d151df5757
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
    "id": 18,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 98,
    "user_id": 650
  }
}
```



```shell
curl "api.goskive.com/v2/questions/98/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 228d5d634f2837395c7edb1ff68c1f84e9f2ab10784fb98fd24f36d151df5757"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/9
Content-Type: application/json
Authorization: Bearer 60faa0f66921e8ba35ebd415c70cf9cebf29d5e03b44564e3ea9492ae9303036
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 52,
    "user_id": 367
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60faa0f66921e8ba35ebd415c70cf9cebf29d5e03b44564e3ea9492ae9303036"
```
