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
Authorization: Bearer 8875be2d79085417fd60bf60a002046fc53e215dd15724e536828da4641c90ba
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
	-H "Authorization: Bearer 8875be2d79085417fd60bf60a002046fc53e215dd15724e536828da4641c90ba"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 11ade973d4f88111dbc463b987d682fca5fd26f677a58bfaeee15ca5313c26eb
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":95,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":95,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11ade973d4f88111dbc463b987d682fca5fd26f677a58bfaeee15ca5313c26eb"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer e8d621938a797c4db341822ecc0ec7462e9c4a5b739180a0c6db94854ba43006
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":96,"pinned":true}}
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
    "course_id": 96,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T17:15:21.784Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:15:21.775Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":96,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8d621938a797c4db341822ecc0ec7462e9c4a5b739180a0c6db94854ba43006"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/47/bookmarks
Content-Type: application/json
Authorization: Bearer f488cc8c8ce09a39da7372cf79f1ae6b03b6cd430c3a581c6d1bf79030d86988
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
    "bookmarkable_id": 47,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/47/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f488cc8c8ce09a39da7372cf79f1ae6b03b6cd430c3a581c6d1bf79030d86988"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/25/votes
Content-Type: application/json
Authorization: Bearer 353f90619ec00d4655b8b7165f33b30eb608ee7bbf0b3cfa5ec08265cfb160a4
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 25,
    "user_id": 202
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/25/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 353f90619ec00d4655b8b7165f33b30eb608ee7bbf0b3cfa5ec08265cfb160a4"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/95/bookmarks
Content-Type: application/json
Authorization: Bearer 3d4b9331b9df396d62702746a020ca6d111450138098f2383dff2d0523712867
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
    "bookmarkable_id": 95,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d4b9331b9df396d62702746a020ca6d111450138098f2383dff2d0523712867"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/96/votes
Content-Type: application/json
Authorization: Bearer cb65c9b9f9f76c79beb50b16414169231d9d1ccefe83d916b94deadde9d55ad6
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 96,
    "user_id": 611
  }
}
```



```shell
curl "api.goskive.com/v2/questions/96/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb65c9b9f9f76c79beb50b16414169231d9d1ccefe83d916b94deadde9d55ad6"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/13
Content-Type: application/json
Authorization: Bearer cacadfdcddf2ba343d2ea8a34c9849f1f6e97031ec1f91891ac6a2a9b9376b44
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 60,
    "user_id": 359
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cacadfdcddf2ba343d2ea8a34c9849f1f6e97031ec1f91891ac6a2a9b9376b44"
```
