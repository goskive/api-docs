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
Authorization: Bearer dc19c6a3bcdd598c7423bde9a7c53ec4b420c59a2b409dc4b026adcfb94e133d
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
	-H "Authorization: Bearer dc19c6a3bcdd598c7423bde9a7c53ec4b420c59a2b409dc4b026adcfb94e133d"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer fef75dcc6518929ffcfe853af431121b437bcb70f44cd8b72b3aa125abb44589
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":250,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":250,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fef75dcc6518929ffcfe853af431121b437bcb70f44cd8b72b3aa125abb44589"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer ec930aa10214426624ee0427d3759dbb9b57a407e4e7c69d23cd047197de2115
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":251,"pinned":true}}
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
    "course_id": 251,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T20:32:37.162Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:32:37.154Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":251,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec930aa10214426624ee0427d3759dbb9b57a407e4e7c69d23cd047197de2115"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer bcc3f1116eb04ffb2788d382749a1d449f43846eb014b76bf47e04bca6a0759d
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
    "bookmarkable_id": 95,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcc3f1116eb04ffb2788d382749a1d449f43846eb014b76bf47e04bca6a0759d"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/48/votes
Content-Type: application/json
Authorization: Bearer 96279d46a92f61316b64f247d79be3b43ae4d9844e39eb0afc952f8b37112fda
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
    "id": 8,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 48,
    "user_id": 451
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/48/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96279d46a92f61316b64f247d79be3b43ae4d9844e39eb0afc952f8b37112fda"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/8/bookmarks
Content-Type: application/json
Authorization: Bearer 554c038c893c50538e3367d8934133993fd0069654acd11dff3771132bbda590
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
    "bookmarkable_id": 8,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/8/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 554c038c893c50538e3367d8934133993fd0069654acd11dff3771132bbda590"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/57/votes
Content-Type: application/json
Authorization: Bearer 72fbe6893f45136c6963038d771a9a84787dc0fda2eb12a668bb03642d0f8a68
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
    "id": 12,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 57,
    "user_id": 496
  }
}
```



```shell
curl "api.goskive.com/v2/questions/57/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72fbe6893f45136c6963038d771a9a84787dc0fda2eb12a668bb03642d0f8a68"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/11
Content-Type: application/json
Authorization: Bearer 1b72def9ac3c10eac3937300d226d11df90d3258466f2699f4c59460338bd091
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 56,
    "user_id": 462
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b72def9ac3c10eac3937300d226d11df90d3258466f2699f4c59460338bd091"
```
