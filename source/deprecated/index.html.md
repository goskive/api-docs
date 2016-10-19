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
Authorization: Bearer b29f4455469702b599d2fc8ccfe06a802ed559f60d29dcba2693d007e179a248
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
	-H "Authorization: Bearer b29f4455469702b599d2fc8ccfe06a802ed559f60d29dcba2693d007e179a248"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer fd7f1724d061e6880215d0830cd2e42b9b70954d49ae8fcf874253dbf34ef784
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":118,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":118,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd7f1724d061e6880215d0830cd2e42b9b70954d49ae8fcf874253dbf34ef784"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c58eadd7f8625e6d0c4b63344d321e3e0bdc341c8c286bf9c20d5ed8de58c6fa
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":119,"pinned":true}}
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
    "course_id": 119,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T08:04:46.073Z",
    "course_published": true,
    "updated_at": "2016-10-19T08:04:46.065Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":119,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c58eadd7f8625e6d0c4b63344d321e3e0bdc341c8c286bf9c20d5ed8de58c6fa"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/91/bookmarks
Content-Type: application/json
Authorization: Bearer eb46a56e02091ab0e7dfc02597839fc5c5214f1e317f4de1031e7f586c00863f
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
    "id": 7,
    "bookmarkable_id": 91,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb46a56e02091ab0e7dfc02597839fc5c5214f1e317f4de1031e7f586c00863f"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/36/votes
Content-Type: application/json
Authorization: Bearer 1a49c7ee8c05f70842990867c0917369032e76381602300a2e2f26e84bc0269a
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
    "votable_id": 36,
    "user_id": 492
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a49c7ee8c05f70842990867c0917369032e76381602300a2e2f26e84bc0269a"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/67/bookmarks
Content-Type: application/json
Authorization: Bearer 90341414aa0917ee2e6c5ed92c86d40a84534d691b96518bdf186f491701388c
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
    "id": 5,
    "bookmarkable_id": 67,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/67/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90341414aa0917ee2e6c5ed92c86d40a84534d691b96518bdf186f491701388c"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer 52163ea7e9bafd09d4f3d63edc5fe04977b917f979171d85bb3900dc47cd84ca
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
    "votable_id": 3,
    "user_id": 15
  }
}
```



```shell
curl "api.goskive.com/v2/questions/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52163ea7e9bafd09d4f3d63edc5fe04977b917f979171d85bb3900dc47cd84ca"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/5
Content-Type: application/json
Authorization: Bearer 1105fcb9fb33824f6fcfce615d991ce4b4ab3d87bca15d559c3d8b3d78b491ac
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
    "votable_id": 4,
    "user_id": 22
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1105fcb9fb33824f6fcfce615d991ce4b4ab3d87bca15d559c3d8b3d78b491ac"
```
