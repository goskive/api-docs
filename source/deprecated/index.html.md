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
Authorization: Bearer 90abf3b8ba5b858156fb9320c577a1831863c214e2506d34f2c04ff6f8e88ff4
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
	-H "Authorization: Bearer 90abf3b8ba5b858156fb9320c577a1831863c214e2506d34f2c04ff6f8e88ff4"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3056f4b4f02ccd5042a8ab3fb64209b4602d1c6088b841a54b185fc9107c6ee4
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":301,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3056f4b4f02ccd5042a8ab3fb64209b4602d1c6088b841a54b185fc9107c6ee4"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 06a7b163d1fd654bdd232bc5ffb012c28abfdefd18b501251c5e02d14a2db5bf
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":302,"pinned":true}}
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
    "course_id": 302,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T12:29:55.273Z",
    "course_published": true,
    "updated_at": "2016-10-26T12:29:55.265Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":302,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06a7b163d1fd654bdd232bc5ffb012c28abfdefd18b501251c5e02d14a2db5bf"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer c4280ba849446b15a2f096d47f85bd54800e3907097025c3b46f0eff66e63b6d
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
    "bookmarkable_id": 95,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4280ba849446b15a2f096d47f85bd54800e3907097025c3b46f0eff66e63b6d"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/61/votes
Content-Type: application/json
Authorization: Bearer ce61952ddfec6211c7cc2fb421e25e8f1a8d139644c698519544e4a556f5dffe
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 61,
    "user_id": 410
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/61/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce61952ddfec6211c7cc2fb421e25e8f1a8d139644c698519544e4a556f5dffe"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/4/bookmarks
Content-Type: application/json
Authorization: Bearer 62a6a0d5b4528bffb59effc4dbeaabe08b1358b0888d89e95696ed08814e7e2b
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
    "bookmarkable_id": 4,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/4/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62a6a0d5b4528bffb59effc4dbeaabe08b1358b0888d89e95696ed08814e7e2b"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/20/votes
Content-Type: application/json
Authorization: Bearer 578f78c9a6773c7f918ed7fe432e31e2d82452825bd2ad0d6d1ea93d3541c776
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
    "id": 3,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 20,
    "user_id": 160
  }
}
```



```shell
curl "api.goskive.com/v2/questions/20/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 578f78c9a6773c7f918ed7fe432e31e2d82452825bd2ad0d6d1ea93d3541c776"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer 648dd0cbc3e7aaf6fd18c6552bbc14e2b43cf24abf83e3de5051bb4ce71bdb44
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
    "votable_id": 102,
    "user_id": 737
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 648dd0cbc3e7aaf6fd18c6552bbc14e2b43cf24abf83e3de5051bb4ce71bdb44"
```
