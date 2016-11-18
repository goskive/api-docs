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
Authorization: Bearer 4f3882ebc39fd397bf540f435dd38fe793edf816be0b23c083a15e91bbe2f6af
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
	-H "Authorization: Bearer 4f3882ebc39fd397bf540f435dd38fe793edf816be0b23c083a15e91bbe2f6af"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 53cf1c471d92e79f48b5e758bb79a8edff09ece0758f9d88961a43b406a891c5
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":139,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":139,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53cf1c471d92e79f48b5e758bb79a8edff09ece0758f9d88961a43b406a891c5"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer ea086fa0426162dc228efca2fa56381bb78154b895deff9376963030fb365e95
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":138,"pinned":true}}
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
    "course_id": 138,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-18T10:56:15.099Z",
    "course_published": true,
    "updated_at": "2016-11-18T10:56:15.091Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":138,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea086fa0426162dc228efca2fa56381bb78154b895deff9376963030fb365e95"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/8/bookmarks
Content-Type: application/json
Authorization: Bearer bde9932825234847aaa92e8cfe6d865753eb971dee65cb6cab6b7f103ee083ba
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
    "bookmarkable_id": 8,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bde9932825234847aaa92e8cfe6d865753eb971dee65cb6cab6b7f103ee083ba"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/81/votes
Content-Type: application/json
Authorization: Bearer d63ba72237221dcfcab6a68fcd52c74d0e9f51b0305edf2b36728ad760cfe7be
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
    "votable_id": 81,
    "user_id": 631
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/81/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d63ba72237221dcfcab6a68fcd52c74d0e9f51b0305edf2b36728ad760cfe7be"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/100/bookmarks
Content-Type: application/json
Authorization: Bearer 62e8c6573fa6f18894115581ba3c6068d28358621613bc1284fb092ceaca2e4e
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
    "bookmarkable_id": 100,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/100/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62e8c6573fa6f18894115581ba3c6068d28358621613bc1284fb092ceaca2e4e"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/7/votes
Content-Type: application/json
Authorization: Bearer 7724090f68341e5507a815faf25766b54ebc24f0f308e0ff21bd49c8ca3abd35
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
    "votable_id": 7,
    "user_id": 56
  }
}
```



```shell
curl "api.goskive.com/v2/questions/7/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7724090f68341e5507a815faf25766b54ebc24f0f308e0ff21bd49c8ca3abd35"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/23
Content-Type: application/json
Authorization: Bearer f184d1f959b4b8cecb05fdfe0b829cb5cf23588320c9242f667ee528502c1992
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 134,
    "user_id": 961
  }
}
```



```shell
curl "api.goskive.com/v2/votes/23" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f184d1f959b4b8cecb05fdfe0b829cb5cf23588320c9242f667ee528502c1992"
```
