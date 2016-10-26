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
Authorization: Bearer ca5289a275a0ee9f8dcd0922a7b81a09aa00fc5dffb939df870024e03f8e49ed
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
	-H "Authorization: Bearer ca5289a275a0ee9f8dcd0922a7b81a09aa00fc5dffb939df870024e03f8e49ed"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4e5e8f0017aaf5dc17e2ef450a7231441789653b900b612371412cc863a5358b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":300,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":300,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e5e8f0017aaf5dc17e2ef450a7231441789653b900b612371412cc863a5358b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2395cf6b4768b1ae72819c6b83a1e3bdca65a04a97efec57dcbace56f19e23b3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":301,"pinned":true}}
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
    "course_id": 301,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T17:19:51.109Z",
    "course_published": true,
    "updated_at": "2016-10-26T17:19:51.097Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":301,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2395cf6b4768b1ae72819c6b83a1e3bdca65a04a97efec57dcbace56f19e23b3"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/88/bookmarks
Content-Type: application/json
Authorization: Bearer 9e50b951e609469b0bedb07ee7a9d8a398a1fad7f570e22e024e527b1cabb09e
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
    "bookmarkable_id": 88,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/88/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e50b951e609469b0bedb07ee7a9d8a398a1fad7f570e22e024e527b1cabb09e"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/41/votes
Content-Type: application/json
Authorization: Bearer 124233f24a5dfc0e3e4fd92783f7e434d132ef7b595cee0ed172095e49488def
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 41,
    "user_id": 293
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/41/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 124233f24a5dfc0e3e4fd92783f7e434d132ef7b595cee0ed172095e49488def"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/134/bookmarks
Content-Type: application/json
Authorization: Bearer d35707b02c684b22cbf49395c23f99e545545be71b7ae0e77ffb753c4f3d527f
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
    "id": 9,
    "bookmarkable_id": 134,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d35707b02c684b22cbf49395c23f99e545545be71b7ae0e77ffb753c4f3d527f"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/11/votes
Content-Type: application/json
Authorization: Bearer c9ae81241a3085f28b5541c30cf5c9a7c6c84993ebd7a7a2b7f52d0dba7a000f
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 11,
    "user_id": 120
  }
}
```



```shell
curl "api.goskive.com/v2/questions/11/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9ae81241a3085f28b5541c30cf5c9a7c6c84993ebd7a7a2b7f52d0dba7a000f"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/3
Content-Type: application/json
Authorization: Bearer 508e0d32985a964ea4f0935979ad50b8f7b9ce71a37ed756122a8d4471a89b42
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
    "id": 3,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 7,
    "user_id": 103
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 508e0d32985a964ea4f0935979ad50b8f7b9ce71a37ed756122a8d4471a89b42"
```
