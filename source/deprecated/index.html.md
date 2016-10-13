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
Authorization: Bearer 4e6f79b1c11baac059b254ca387fde6fff1ad4293452c1fc06ae6fdfb9e8e26a
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
	-H "Authorization: Bearer 4e6f79b1c11baac059b254ca387fde6fff1ad4293452c1fc06ae6fdfb9e8e26a"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 809829d3c10f8a64ec9be66260b1b7be37952040222e663334939e07d11c7c14
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":121,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":121,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 809829d3c10f8a64ec9be66260b1b7be37952040222e663334939e07d11c7c14"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 65104b2121a8cc1d5d629da677abd59e053802a7ae4210ba4174716001185d11
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":120,"pinned":true}}
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
    "course_id": 120,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T13:40:00.384Z",
    "course_published": true,
    "updated_at": "2016-10-13T13:40:00.374Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":120,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65104b2121a8cc1d5d629da677abd59e053802a7ae4210ba4174716001185d11"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/58/bookmarks
Content-Type: application/json
Authorization: Bearer e4e76f4dab2426a8a5ca5cddbe4cb2cf620fbd04c5e6570acf29fb35409adcb9
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
    "bookmarkable_id": 58,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/58/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4e76f4dab2426a8a5ca5cddbe4cb2cf620fbd04c5e6570acf29fb35409adcb9"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/51/votes
Content-Type: application/json
Authorization: Bearer 50ed078003df45bf69aafa41131c01ddd57375485e74e4b0473603ebe677e478
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
    "id": 9,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 51,
    "user_id": 441
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/51/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50ed078003df45bf69aafa41131c01ddd57375485e74e4b0473603ebe677e478"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/79/bookmarks
Content-Type: application/json
Authorization: Bearer 7af1e148ea0d86b1f3e4a85d43a8558a807d9ba2fea238b66b5df9ef133fd8a1
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
    "id": 8,
    "bookmarkable_id": 79,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/79/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7af1e148ea0d86b1f3e4a85d43a8558a807d9ba2fea238b66b5df9ef133fd8a1"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/101/votes
Content-Type: application/json
Authorization: Bearer 0bd3070bc05c61a459409054491a984ccf4001b5019bd7bf46ec79abd21bdeb9
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
    "votable_id": 101,
    "user_id": 873
  }
}
```



```shell
curl "api.goskive.com/v2/questions/101/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bd3070bc05c61a459409054491a984ccf4001b5019bd7bf46ec79abd21bdeb9"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/4
Content-Type: application/json
Authorization: Bearer 4c8028a09956471a586acdb5ee7df8fec955a19bebe42847f93ccccefa423b05
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 13,
    "user_id": 142
  }
}
```



```shell
curl "api.goskive.com/v2/votes/4" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c8028a09956471a586acdb5ee7df8fec955a19bebe42847f93ccccefa423b05"
```
