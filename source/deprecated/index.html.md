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
Authorization: Bearer 0acdef0e938eb7f809eed60cb7dd159ba7d32b8aab5188ff4226b9a939a67f54
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
	-H "Authorization: Bearer 0acdef0e938eb7f809eed60cb7dd159ba7d32b8aab5188ff4226b9a939a67f54"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c17b4cbafc460a2261385e7ae1f94e7f6d17d3888e50d4c5619b78cf040b41c6
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":145,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":145,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c17b4cbafc460a2261385e7ae1f94e7f6d17d3888e50d4c5619b78cf040b41c6"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 611a0466dea76dbe91153519b23a7271d3633d31cadcdb4fa72121b60b4f246e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":144,"pinned":true}}
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
    "course_id": 144,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T14:00:12.989Z",
    "course_published": true,
    "updated_at": "2016-10-13T14:00:12.979Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":144,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 611a0466dea76dbe91153519b23a7271d3633d31cadcdb4fa72121b60b4f246e"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/81/bookmarks
Content-Type: application/json
Authorization: Bearer 8ecb9a33d765ce6ed2be8dc0c0e6bbf924169c62ef68f4cd2bb4ead930369510
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
    "id": 8,
    "bookmarkable_id": 81,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/81/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ecb9a33d765ce6ed2be8dc0c0e6bbf924169c62ef68f4cd2bb4ead930369510"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/29/votes
Content-Type: application/json
Authorization: Bearer db540cf2a29b5a5753b6f6bf6e61015be312a18d7117628a2391a8d86fe0c2bd
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
    "votable_id": 29,
    "user_id": 83
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db540cf2a29b5a5753b6f6bf6e61015be312a18d7117628a2391a8d86fe0c2bd"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/97/bookmarks
Content-Type: application/json
Authorization: Bearer 021ed47dabc95732d5c3f515d3f64cbec5f1c7fe457534452a7dcc97bc38476d
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
    "id": 7,
    "bookmarkable_id": 97,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/97/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 021ed47dabc95732d5c3f515d3f64cbec5f1c7fe457534452a7dcc97bc38476d"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/80/votes
Content-Type: application/json
Authorization: Bearer 465f4c8af4288f142c7d59a268a62e268d29c7c880df30a5f6665c49f430ea5b
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 80,
    "user_id": 527
  }
}
```



```shell
curl "api.goskive.com/v2/questions/80/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 465f4c8af4288f142c7d59a268a62e268d29c7c880df30a5f6665c49f430ea5b"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/20
Content-Type: application/json
Authorization: Bearer c5eebdd7d70ddf8d1cbe537b11dfeda6cae670f63e7e833e46fd42d5b6b664e4
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 132,
    "user_id": 953
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5eebdd7d70ddf8d1cbe537b11dfeda6cae670f63e7e833e46fd42d5b6b664e4"
```
