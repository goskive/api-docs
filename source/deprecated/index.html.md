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
Authorization: Bearer deb61d0014258fc7fd5fc903c43bd5ec17a2937b897136a941b7a7eb92b608d4
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
	-H "Authorization: Bearer deb61d0014258fc7fd5fc903c43bd5ec17a2937b897136a941b7a7eb92b608d4"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 060ce0979407be4978d1b49f2d1765e296d43998bb2fb18fee1e7a2b00502cad
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":293,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":293,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 060ce0979407be4978d1b49f2d1765e296d43998bb2fb18fee1e7a2b00502cad"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 64ab053afc0944b8d9ce90b82c4713f46b0ccb655dfa6c54459d33ea8dbeb382
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
201 Created
```


```json
{
  "user_course": {
    "id": 12,
    "course_id": 292,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-22T08:05:35.209Z",
    "course_published": true,
    "updated_at": "2016-09-22T08:05:35.200Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":292,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64ab053afc0944b8d9ce90b82c4713f46b0ccb655dfa6c54459d33ea8dbeb382"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/82/bookmarks
Content-Type: application/json
Authorization: Bearer 174d2319462de8231046e18e1e715978a54d4d9765f2f3f3a08845192137cb31
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
    "bookmarkable_id": 82,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 174d2319462de8231046e18e1e715978a54d4d9765f2f3f3a08845192137cb31"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/83/votes
Content-Type: application/json
Authorization: Bearer b27c8b558719699bd6a7b8764782ccfcedbf708e216b05cbdb80fae95df61ae2
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 83,
    "user_id": 781
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b27c8b558719699bd6a7b8764782ccfcedbf708e216b05cbdb80fae95df61ae2"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/91/bookmarks
Content-Type: application/json
Authorization: Bearer 2006b0ecaddadcf4c63cdde700d29f6a1cc94fb16fa50c3de10ef01a7271d748
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
    "bookmarkable_id": 91,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2006b0ecaddadcf4c63cdde700d29f6a1cc94fb16fa50c3de10ef01a7271d748"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/11/votes
Content-Type: application/json
Authorization: Bearer 5a3171eecada07e3b77bba212a057ce2564e0a1c2820051a083cce9a5f1501db
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
    "votable_id": 11,
    "user_id": 129
  }
}
```



```shell
curl "api.goskive.com/v2/questions/11/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a3171eecada07e3b77bba212a057ce2564e0a1c2820051a083cce9a5f1501db"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer 374d41dea9643d0711b2fc53cc8288314ed260ac8ae3672ce246bfe734c62743
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 90,
    "user_id": 622
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 374d41dea9643d0711b2fc53cc8288314ed260ac8ae3672ce246bfe734c62743"
```
