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
Authorization: Bearer 7adecb076797194c6c0538594df1f5715fc028b3474c98548f3e1eddeebfc496
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
	-H "Authorization: Bearer 7adecb076797194c6c0538594df1f5715fc028b3474c98548f3e1eddeebfc496"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b0fc2505fd80751e3a4bad9408e9ea280c6cd0127a35494488b4f3094481e4a9
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":233,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":233,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0fc2505fd80751e3a4bad9408e9ea280c6cd0127a35494488b4f3094481e4a9"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4e08fb7b6e324d7f429a92b4ca96e2c699f58e3a55fc06b7f589004066984bc7
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":232,"pinned":true}}
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
    "course_id": 232,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T16:35:33.010Z",
    "course_published": true,
    "updated_at": "2016-10-18T16:35:33.002Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":232,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e08fb7b6e324d7f429a92b4ca96e2c699f58e3a55fc06b7f589004066984bc7"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/16/bookmarks
Content-Type: application/json
Authorization: Bearer f839f7465bb55ed502c4b4d2620c72f83b6753a5882a5782d03e591b435a2b6e
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
    "bookmarkable_id": 16,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/16/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f839f7465bb55ed502c4b4d2620c72f83b6753a5882a5782d03e591b435a2b6e"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/26/votes
Content-Type: application/json
Authorization: Bearer 866b95e1f292dea078e7e787f142cde277d75444ff1594b1c8430d8e523f76e0
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 26,
    "user_id": 399
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/26/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 866b95e1f292dea078e7e787f142cde277d75444ff1594b1c8430d8e523f76e0"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/47/bookmarks
Content-Type: application/json
Authorization: Bearer 11619ed5aa2316a4c6219560ae2fb6b1ee63b3cf1a1596e1d0be9a45674fbe58
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
    "id": 4,
    "bookmarkable_id": 47,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/47/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11619ed5aa2316a4c6219560ae2fb6b1ee63b3cf1a1596e1d0be9a45674fbe58"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/134/votes
Content-Type: application/json
Authorization: Bearer c4931be73cfa2d6da41cc3ac4e87031e9d268c52c3b70dacfcab1eb6fc25eadb
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
    "votable_id": 134,
    "user_id": 951
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4931be73cfa2d6da41cc3ac4e87031e9d268c52c3b70dacfcab1eb6fc25eadb"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/4
Content-Type: application/json
Authorization: Bearer 74bb414913aeca3a15303926739ed4730314a477d6d91950510c87e288c00128
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 25,
    "user_id": 218
  }
}
```



```shell
curl "api.goskive.com/v2/votes/4" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74bb414913aeca3a15303926739ed4730314a477d6d91950510c87e288c00128"
```
