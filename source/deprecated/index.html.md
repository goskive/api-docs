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
DELETE /v2/bookmarks/10
Content-Type: application/json
Authorization: Bearer e040f28fccd0e2ff41e6ff9ab07a861e0c4551020cd6328c503a77ba16eacc3d
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e040f28fccd0e2ff41e6ff9ab07a861e0c4551020cd6328c503a77ba16eacc3d"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c9edfccf12707bcd9081f4c0a2dedb791e5ae192285d2ae0ce0d8ff66a60be35
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
	-H "Authorization: Bearer c9edfccf12707bcd9081f4c0a2dedb791e5ae192285d2ae0ce0d8ff66a60be35"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 5192fb515e1efcd9d0a08ca923cbd4d2942e2060787cd358d8c045818b824ab8
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":249,"pinned":true}}
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
    "course_id": 249,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-29T17:22:50.504Z",
    "course_published": true,
    "updated_at": "2016-10-29T17:22:50.496Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":249,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5192fb515e1efcd9d0a08ca923cbd4d2942e2060787cd358d8c045818b824ab8"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/25/bookmarks
Content-Type: application/json
Authorization: Bearer d715a8653e658c0299675a22e3d914103f2079a4691d241d5eace01034de32a7
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
    "bookmarkable_id": 25,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/25/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d715a8653e658c0299675a22e3d914103f2079a4691d241d5eace01034de32a7"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/82/votes
Content-Type: application/json
Authorization: Bearer 045962fa156c1bd361f8c9a060ec950348458d655e6d5c0d82bfeea80c312479
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
    "id": 20,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 82,
    "user_id": 848
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 045962fa156c1bd361f8c9a060ec950348458d655e6d5c0d82bfeea80c312479"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/1/bookmarks
Content-Type: application/json
Authorization: Bearer 1dda6757ada3f8ba848e562eef1904b25c0390167c04112b311e5abd946525d9
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
    "id": 4,
    "bookmarkable_id": 1,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/1/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1dda6757ada3f8ba848e562eef1904b25c0390167c04112b311e5abd946525d9"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/122/votes
Content-Type: application/json
Authorization: Bearer cd7acb958fd777c475e4ad3a13eacc795c7173ca202fea4553d5dfbf49ce1c4d
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
    "id": 19,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 122,
    "user_id": 843
  }
}
```



```shell
curl "api.goskive.com/v2/questions/122/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd7acb958fd777c475e4ad3a13eacc795c7173ca202fea4553d5dfbf49ce1c4d"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/15
Content-Type: application/json
Authorization: Bearer cdc0c7703b093efbec3dfe0680282086ac56d6f65979e948fa3b1d4413f2f3d8
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
    "id": 15,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 111,
    "user_id": 793
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdc0c7703b093efbec3dfe0680282086ac56d6f65979e948fa3b1d4413f2f3d8"
```
