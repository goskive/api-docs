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
DELETE /v2/bookmarks/8
Content-Type: application/json
Authorization: Bearer 80fdf52d506042be18291728a4b1b28c7e6fafcaaf2c928b5afae7621d190128
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80fdf52d506042be18291728a4b1b28c7e6fafcaaf2c928b5afae7621d190128"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer ec395f53f8143b5f1c3e066ab7c3e9567e0e7ad80f99a85145d9ab6acdb5e1b4
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":151,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":151,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec395f53f8143b5f1c3e066ab7c3e9567e0e7ad80f99a85145d9ab6acdb5e1b4"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8c3ee81469a683099b047d489243cdf7e1e1149376f07fde9d99b7e5051fc29f
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":150,"pinned":true}}
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
    "id": 1,
    "course_id": 150,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T19:45:30.811Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:45:30.802Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":150,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c3ee81469a683099b047d489243cdf7e1e1149376f07fde9d99b7e5051fc29f"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/33/bookmarks
Content-Type: application/json
Authorization: Bearer 4b4ba43b106ec1bf0c54c9da796779158b5e4c533df500ddd511212c560c64e1
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
    "id": 6,
    "bookmarkable_id": 33,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/33/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b4ba43b106ec1bf0c54c9da796779158b5e4c533df500ddd511212c560c64e1"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/14/votes
Content-Type: application/json
Authorization: Bearer c0e53f44da898d870a30af60014afb0cf980701771dafc4830a8d4313d3cdd90
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
    "votable_id": 14,
    "user_id": 281
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/14/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0e53f44da898d870a30af60014afb0cf980701771dafc4830a8d4313d3cdd90"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/93/bookmarks
Content-Type: application/json
Authorization: Bearer 975d44e166a32646958f2fd85a4ff63ec34ae114595f099335fa609f60f92327
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
    "bookmarkable_id": 93,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/93/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 975d44e166a32646958f2fd85a4ff63ec34ae114595f099335fa609f60f92327"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/32/votes
Content-Type: application/json
Authorization: Bearer 00d51cd855380b40e3bdf4b31f5b1a9f880f4ef7f14b5b11adebee4050956d81
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 32,
    "user_id": 138
  }
}
```



```shell
curl "api.goskive.com/v2/questions/32/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00d51cd855380b40e3bdf4b31f5b1a9f880f4ef7f14b5b11adebee4050956d81"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/12
Content-Type: application/json
Authorization: Bearer 4494f9e8e33a771294407b197eecb883dcd8045a0633c7d9f9c216e92ca373c7
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 56,
    "user_id": 370
  }
}
```



```shell
curl "api.goskive.com/v2/votes/12" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4494f9e8e33a771294407b197eecb883dcd8045a0633c7d9f9c216e92ca373c7"
```
