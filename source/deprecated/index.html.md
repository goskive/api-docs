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
Authorization: Bearer 241df4f94070d9bc200882ad22d3711f55858ca4dc1e0c6b22d977b4ea8fb766
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
	-H "Authorization: Bearer 241df4f94070d9bc200882ad22d3711f55858ca4dc1e0c6b22d977b4ea8fb766"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8406cd83a0cc238c81a84a3f57992fd67bde3f63cbd1365085e27d04e5e47616
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":47,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":47,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8406cd83a0cc238c81a84a3f57992fd67bde3f63cbd1365085e27d04e5e47616"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer d0278e464c3adf6e35f6a9d3813a185e305b2158b97ce7b04ac9f09951823528
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":46,"pinned":true}}
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
    "course_id": 46,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T11:35:24.398Z",
    "course_published": true,
    "updated_at": "2016-10-14T11:35:24.388Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":46,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0278e464c3adf6e35f6a9d3813a185e305b2158b97ce7b04ac9f09951823528"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/84/bookmarks
Content-Type: application/json
Authorization: Bearer dc98cd1df66c170485308bc70bc0a6e30656317bc584d58543cdbbadc6a81811
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
    "bookmarkable_id": 84,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc98cd1df66c170485308bc70bc0a6e30656317bc584d58543cdbbadc6a81811"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/45/votes
Content-Type: application/json
Authorization: Bearer cd2abb426ede99c3377b3fb02523e1f1eb7f59e5ec7fc32a11294f7a3d1e36a2
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
    "id": 11,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 45,
    "user_id": 254
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/45/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd2abb426ede99c3377b3fb02523e1f1eb7f59e5ec7fc32a11294f7a3d1e36a2"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/47/bookmarks
Content-Type: application/json
Authorization: Bearer b2edb7a6b3a78b9d5f3dc6155fdb0853a4aac06ba3129c7e80202be699cb29ec
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
    "id": 6,
    "bookmarkable_id": 47,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/47/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2edb7a6b3a78b9d5f3dc6155fdb0853a4aac06ba3129c7e80202be699cb29ec"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/134/votes
Content-Type: application/json
Authorization: Bearer 85a3b3ce78b7aa3c158a4a077abd80b35b1e34d86c7dfa7ec26a0f3bde517790
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
	-H "Authorization: Bearer 85a3b3ce78b7aa3c158a4a077abd80b35b1e34d86c7dfa7ec26a0f3bde517790"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/3
Content-Type: application/json
Authorization: Bearer cec087e77ba95af14e4596cfbf007d01cbca919d7e358225471a232e6323ca5a
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
    "id": 3,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 4,
    "user_id": 13
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cec087e77ba95af14e4596cfbf007d01cbca919d7e358225471a232e6323ca5a"
```
