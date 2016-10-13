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
Authorization: Bearer 4d8cbb334f2d7ddb6c803782bd664671e2156abfd34189cd13bf7f4e392b4e22
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
	-H "Authorization: Bearer 4d8cbb334f2d7ddb6c803782bd664671e2156abfd34189cd13bf7f4e392b4e22"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4bf1660a61c6e0efea2a78207d302d088a7907a5f59a9f7d1fdba4a5b9ff466b
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":112,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":112,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4bf1660a61c6e0efea2a78207d302d088a7907a5f59a9f7d1fdba4a5b9ff466b"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6a296c2e49745cbda76e2f3ec7353b369bfdb32ab125c4ddeed8883f0c228a0a
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":113,"pinned":true}}
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
    "course_id": 113,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T12:52:07.476Z",
    "course_published": true,
    "updated_at": "2016-10-13T12:52:07.467Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":113,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a296c2e49745cbda76e2f3ec7353b369bfdb32ab125c4ddeed8883f0c228a0a"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/76/bookmarks
Content-Type: application/json
Authorization: Bearer 91b903d04f7a32f8279773f7cf078419d2f7e48bf66d68ed74e5136496d148e1
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
    "id": 4,
    "bookmarkable_id": 76,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/76/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91b903d04f7a32f8279773f7cf078419d2f7e48bf66d68ed74e5136496d148e1"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/19/votes
Content-Type: application/json
Authorization: Bearer 458fafc0b5e68f70dd5c3ded31a5ca571c941be6ff2dbbf8f775284a84bc8e39
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 19,
    "user_id": 175
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/19/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 458fafc0b5e68f70dd5c3ded31a5ca571c941be6ff2dbbf8f775284a84bc8e39"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/1/bookmarks
Content-Type: application/json
Authorization: Bearer ad713aef103409ed0f88b36454751f349e58aaf28ca4ce398fe0c00cb1be56a6
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
    "bookmarkable_id": 1,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad713aef103409ed0f88b36454751f349e58aaf28ca4ce398fe0c00cb1be56a6"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/134/votes
Content-Type: application/json
Authorization: Bearer 7825fb2ed16b90cf3130584a7a511f522d36c2ffe4114c5e4ee3324ad7b0a5a0
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
    "user_id": 962
  }
}
```



```shell
curl "api.goskive.com/v2/questions/134/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7825fb2ed16b90cf3130584a7a511f522d36c2ffe4114c5e4ee3324ad7b0a5a0"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/9
Content-Type: application/json
Authorization: Bearer 4e432707c43cc0e2a81a380ede6829804f88bcd130931be3301be0529b015a13
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
    "votable_id": 79,
    "user_id": 491
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e432707c43cc0e2a81a380ede6829804f88bcd130931be3301be0529b015a13"
```
