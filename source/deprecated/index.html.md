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
DELETE /v2/bookmarks/3
Content-Type: application/json
Authorization: Bearer 9b9a9040fbf1f94e1a75b869f5ca3ad840fdd0cb1729d4aae3493eb7acb95de5
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b9a9040fbf1f94e1a75b869f5ca3ad840fdd0cb1729d4aae3493eb7acb95de5"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b02385b1b1bf35b137b05280389157d157efb3da0cce9b2b9dd6d291dc443893
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":23,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":23,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b02385b1b1bf35b137b05280389157d157efb3da0cce9b2b9dd6d291dc443893"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 52c5a998f4fa1f5f5a7ff4f0769d884a12479a524917bcfda331543e09a98257
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":24,"pinned":true}}
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
    "course_id": 24,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T20:44:11.085Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:44:11.077Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":24,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52c5a998f4fa1f5f5a7ff4f0769d884a12479a524917bcfda331543e09a98257"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/12/bookmarks
Content-Type: application/json
Authorization: Bearer fcf2ba33a1d58a550ac4cf64098f42a429dd3bb83ddcdbef825445f0823e9b35
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
    "bookmarkable_id": 12,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/12/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcf2ba33a1d58a550ac4cf64098f42a429dd3bb83ddcdbef825445f0823e9b35"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/29/votes
Content-Type: application/json
Authorization: Bearer e5598cdab987211055fc5f5c726a456f4d90a7deac65621cbe8e2dbfb2265775
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 29,
    "user_id": 448
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5598cdab987211055fc5f5c726a456f4d90a7deac65621cbe8e2dbfb2265775"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/11/bookmarks
Content-Type: application/json
Authorization: Bearer f49086252caf26cf1a9b68fdea14da734929a48330e9212690cbe35f08834996
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
    "id": 1,
    "bookmarkable_id": 11,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/11/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f49086252caf26cf1a9b68fdea14da734929a48330e9212690cbe35f08834996"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/28/votes
Content-Type: application/json
Authorization: Bearer f1620872ec9dce5898335aa08dc97435ef754fb65300aff2361ab42e2506f5e0
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
    "votable_id": 28,
    "user_id": 179
  }
}
```



```shell
curl "api.goskive.com/v2/questions/28/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1620872ec9dce5898335aa08dc97435ef754fb65300aff2361ab42e2506f5e0"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/5
Content-Type: application/json
Authorization: Bearer 0f618eed4332d7f8d8af9b04517ed30ae947434de46c673f20d0c5972524d148
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 38,
    "user_id": 241
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f618eed4332d7f8d8af9b04517ed30ae947434de46c673f20d0c5972524d148"
```
