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
DELETE /v2/bookmarks/7
Content-Type: application/json
Authorization: Bearer bc34b9146afc427b4d14cdd15d5443a7eb3e4c8952b70a06869d82c26884e92b
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc34b9146afc427b4d14cdd15d5443a7eb3e4c8952b70a06869d82c26884e92b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0909082a0d5ca03feafd99d8e30cbb30f24585a6d3f68ee6170f1dfabc211116
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":292,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":292,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0909082a0d5ca03feafd99d8e30cbb30f24585a6d3f68ee6170f1dfabc211116"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0275e7adae956613c40164314543b26a98f1be5271c151a356a53e65f9883631
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":291,"pinned":true}}
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
    "id": 8,
    "course_id": 291,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T09:10:41.059Z",
    "course_published": true,
    "updated_at": "2016-12-08T09:10:41.054Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":291,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0275e7adae956613c40164314543b26a98f1be5271c151a356a53e65f9883631"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/76/bookmarks
Content-Type: application/json
Authorization: Bearer d805ed4ccd8953abd4df8fce9fc8cc16f27bbb1785e9f25bda78e35bbc8fbd57
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
    "id": 5,
    "bookmarkable_id": 76,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/76/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d805ed4ccd8953abd4df8fce9fc8cc16f27bbb1785e9f25bda78e35bbc8fbd57"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/70/votes
Content-Type: application/json
Authorization: Bearer afcf4b0c54c2b0141249f98a6d75583dbd17af1af98f978dd79a63939cbe603b
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
    "id": 16,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 70,
    "user_id": 652
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/70/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afcf4b0c54c2b0141249f98a6d75583dbd17af1af98f978dd79a63939cbe603b"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/125/bookmarks
Content-Type: application/json
Authorization: Bearer 36a409c787456ba17b65b765c2e7c19021d4a5c947e8cc090a725d850e0fe72a
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
    "bookmarkable_id": 125,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/125/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36a409c787456ba17b65b765c2e7c19021d4a5c947e8cc090a725d850e0fe72a"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/126/votes
Content-Type: application/json
Authorization: Bearer 9713d39db04b407fb3a45b9d00e556accf2f45cbbc64c1a66902852c90870256
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 126,
    "user_id": 928
  }
}
```



```shell
curl "api.goskive.com/v2/questions/126/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9713d39db04b407fb3a45b9d00e556accf2f45cbbc64c1a66902852c90870256"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/1
Content-Type: application/json
Authorization: Bearer 6f82a20dad93e3cf695bb16da65aaf1a250b4e8b5e1c9c47842344185a684457
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 27,
    "user_id": 62
  }
}
```



```shell
curl "api.goskive.com/v2/votes/1" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f82a20dad93e3cf695bb16da65aaf1a250b4e8b5e1c9c47842344185a684457"
```
