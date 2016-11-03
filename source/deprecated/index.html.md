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
Authorization: Bearer d519b7f6b6ceb6f1d1cb7f4b1eb4450ee72461603d1e935f31368e106493d0c9
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
	-H "Authorization: Bearer d519b7f6b6ceb6f1d1cb7f4b1eb4450ee72461603d1e935f31368e106493d0c9"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 881e0100f5e9749c52cd2143a5e65fedea0c6807fd064a9fd70ce2596b7caad5
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":212,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":212,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 881e0100f5e9749c52cd2143a5e65fedea0c6807fd064a9fd70ce2596b7caad5"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer df300bc6877d5b4d4635019f27627dafe24feca74de769de821b0521eaba7a81
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":213,"pinned":true}}
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
    "course_id": 213,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T11:27:50.607Z",
    "course_published": true,
    "updated_at": "2016-11-03T11:27:50.599Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":213,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df300bc6877d5b4d4635019f27627dafe24feca74de769de821b0521eaba7a81"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/88/bookmarks
Content-Type: application/json
Authorization: Bearer 30778eded47f2eb27ec2caeedcfde2cc7c8217346f84f6cd01f95a033c883454
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
    "id": 9,
    "bookmarkable_id": 88,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/88/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30778eded47f2eb27ec2caeedcfde2cc7c8217346f84f6cd01f95a033c883454"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/95/votes
Content-Type: application/json
Authorization: Bearer efd59d8c8f08332a03ff8daaa919a2956b5ac668df3b7ef189faa2776ac2c86d
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
    "id": 23,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 95,
    "user_id": 983
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer efd59d8c8f08332a03ff8daaa919a2956b5ac668df3b7ef189faa2776ac2c86d"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/72/bookmarks
Content-Type: application/json
Authorization: Bearer d44a4659c9a3ff7310ee1a455678ffbea9e6b0e6b3d6838bf8f61faa5d5d281b
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
    "id": 2,
    "bookmarkable_id": 72,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/72/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d44a4659c9a3ff7310ee1a455678ffbea9e6b0e6b3d6838bf8f61faa5d5d281b"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/88/votes
Content-Type: application/json
Authorization: Bearer c64c14087a8690938187213767b031dabf54b5efba2a92d7937369165c9263d2
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
    "votable_id": 88,
    "user_id": 745
  }
}
```



```shell
curl "api.goskive.com/v2/questions/88/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c64c14087a8690938187213767b031dabf54b5efba2a92d7937369165c9263d2"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/2
Content-Type: application/json
Authorization: Bearer e0b0c668c32a0555694884edf5dfe1ce41b182959aed284b4b7f2fc7ae172081
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
    "id": 2,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 80,
    "user_id": 573
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0b0c668c32a0555694884edf5dfe1ce41b182959aed284b4b7f2fc7ae172081"
```
