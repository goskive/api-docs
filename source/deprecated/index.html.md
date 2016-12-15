---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Bookmarks

## Delete a bookmark

DEPRECATED. Use DELETE /v2/:content_unit_type/:content_unit_id/bookmark instead.

### Request

#### Endpoint

```
DELETE /v2/bookmarks/9
Content-Type: application/json
Authorization: Bearer 11b2890c8ca0091039b3e95907ce5a35784fb1cf2dfd07231ac2ebc8c7e57531
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11b2890c8ca0091039b3e95907ce5a35784fb1cf2dfd07231ac2ebc8c7e57531"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2ba8c7e20a0f33b8aa78983574fe3166e97c12729cc8865480433abab09ecbdd
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":73,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":73,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ba8c7e20a0f33b8aa78983574fe3166e97c12729cc8865480433abab09ecbdd"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6a38f6b103680ecd92a20eaad779acfba2b7113bda993a7fe6886fb6d327f947
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":74,"pinned":true}}
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
    "course_id": 74,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T14:27:00.351Z",
    "course_published": true,
    "updated_at": "2016-12-15T14:27:00.346Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":74,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a38f6b103680ecd92a20eaad779acfba2b7113bda993a7fe6886fb6d327f947"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/58/bookmarks
Content-Type: application/json
Authorization: Bearer 09607c09827b0421f0322587929ff6be8b08406fb876ed80da2a12dccdfd42b1
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
    "bookmarkable_id": 58,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/58/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09607c09827b0421f0322587929ff6be8b08406fb876ed80da2a12dccdfd42b1"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/51/votes
Content-Type: application/json
Authorization: Bearer 8db903e9b6fbb9de5eb852511ae0e9a78a79ac34e10c272829b14132684364bd
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
    "votable_id": 51,
    "user_id": 206
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/51/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8db903e9b6fbb9de5eb852511ae0e9a78a79ac34e10c272829b14132684364bd"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/58/bookmarks
Content-Type: application/json
Authorization: Bearer c94560fbbddaffff6c6ac873f6d84a42d8a2f48d5651eb0e03945aaab1db28b3
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
    "bookmarkable_id": 58,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/58/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c94560fbbddaffff6c6ac873f6d84a42d8a2f48d5651eb0e03945aaab1db28b3"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/55/votes
Content-Type: application/json
Authorization: Bearer 69be4e8cd9b6d1667cf84a08ebd77fbfc24632901c9c85339507f8c1411d4a94
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
    "votable_id": 55,
    "user_id": 333
  }
}
```



```shell
curl "api.goskive.com/v2/questions/55/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69be4e8cd9b6d1667cf84a08ebd77fbfc24632901c9c85339507f8c1411d4a94"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/5
Content-Type: application/json
Authorization: Bearer 955a991305347fa574fb9e1406ec635bd72aa2b30157234c55e1dbd1a82207ce
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
    "id": 5,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 132
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 955a991305347fa574fb9e1406ec635bd72aa2b30157234c55e1dbd1a82207ce"
```
