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
Authorization: Bearer 9c98d1349b25e1092e935ccb1f19803f13435a5c3467e86cf2f0beb07892fd1c
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
	-H "Authorization: Bearer 9c98d1349b25e1092e935ccb1f19803f13435a5c3467e86cf2f0beb07892fd1c"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 495196366356a88e46359a396b0ba11a31c155943a8a8045dec6e3dfa3031321
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":267,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":267,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 495196366356a88e46359a396b0ba11a31c155943a8a8045dec6e3dfa3031321"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6a3cb432f6e375ec2297c2ef442eb1ded2ea79945323a4d2a6f37de40d45ca0f
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":266,"pinned":true}}
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
    "id": 4,
    "course_id": 266,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T20:52:26.088Z",
    "course_published": true,
    "updated_at": "2016-12-08T20:52:26.083Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":266,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a3cb432f6e375ec2297c2ef442eb1ded2ea79945323a4d2a6f37de40d45ca0f"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/20/bookmarks
Content-Type: application/json
Authorization: Bearer cd8daa18283169a57a73a4d7e899a9bfffb0e4c2db24f95f4578b207181f1049
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
    "id": 3,
    "bookmarkable_id": 20,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/20/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd8daa18283169a57a73a4d7e899a9bfffb0e4c2db24f95f4578b207181f1049"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/1/votes
Content-Type: application/json
Authorization: Bearer 29d3de88debb1d6e5e7c4228610761be5076b48bcb69affb83229d311ce89b10
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 1,
    "user_id": 21
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/1/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29d3de88debb1d6e5e7c4228610761be5076b48bcb69affb83229d311ce89b10"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/44/bookmarks
Content-Type: application/json
Authorization: Bearer 8c9f75c68e0eeae3dc7083985dfd1b81548479facb122615c883c8da0bd6b08f
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
    "bookmarkable_id": 44,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/44/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c9f75c68e0eeae3dc7083985dfd1b81548479facb122615c883c8da0bd6b08f"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer 0f94d9a7bb9c9a52d9457bbe19945740aa6178dec164ed925e1c3e91c09f0886
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 10
  }
}
```



```shell
curl "api.goskive.com/v2/questions/3/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f94d9a7bb9c9a52d9457bbe19945740aa6178dec164ed925e1c3e91c09f0886"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer d3021663c7266cf338dbfcc7c3df722706aa6bd8f235eee052187eb570b2217c
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
    "votable_id": 48,
    "user_id": 397
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3021663c7266cf338dbfcc7c3df722706aa6bd8f235eee052187eb570b2217c"
```
