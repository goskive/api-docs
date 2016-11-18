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
DELETE /v2/bookmarks/2
Content-Type: application/json
Authorization: Bearer 1501861f0919c1143be03b73440ec7bbf953185349c1cd570a9c5cfe82d16d0b
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1501861f0919c1143be03b73440ec7bbf953185349c1cd570a9c5cfe82d16d0b"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 53049d79864e0cc315d95b2329af1ffd2a6b6c7b8bb300ea8e14617486a2f5e5
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":259,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":259,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53049d79864e0cc315d95b2329af1ffd2a6b6c7b8bb300ea8e14617486a2f5e5"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8e72860e0a5000792fbd1ef0c0bd91045d8d5e423e347c6f2d49ced1fe042154
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":260,"pinned":true}}
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
    "id": 7,
    "course_id": 260,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-18T09:48:40.893Z",
    "course_published": true,
    "updated_at": "2016-11-18T09:48:40.884Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":260,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e72860e0a5000792fbd1ef0c0bd91045d8d5e423e347c6f2d49ced1fe042154"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/18/bookmarks
Content-Type: application/json
Authorization: Bearer 1532f6d1685546a4b86d60d3fd04dae293bb5618ea00d872059edf9724715c3b
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
    "bookmarkable_id": 18,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/18/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1532f6d1685546a4b86d60d3fd04dae293bb5618ea00d872059edf9724715c3b"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/29/votes
Content-Type: application/json
Authorization: Bearer bf9efb89f6c1f196b08ec93a6e9fd5f5fbf5705215454525041be352f931af21
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
    "votable_id": 29,
    "user_id": 329
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf9efb89f6c1f196b08ec93a6e9fd5f5fbf5705215454525041be352f931af21"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/38/bookmarks
Content-Type: application/json
Authorization: Bearer 4aa47d4757b9d57a0f0df07771877f7cf15889f4ec3483e367433e77d693e558
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
    "bookmarkable_id": 38,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/38/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4aa47d4757b9d57a0f0df07771877f7cf15889f4ec3483e367433e77d693e558"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/45/votes
Content-Type: application/json
Authorization: Bearer fadb99c5fe469b3ee303424ab1385dc9337ac475752d81552a88a9b3ef37d04e
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 45,
    "user_id": 343
  }
}
```



```shell
curl "api.goskive.com/v2/questions/45/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fadb99c5fe469b3ee303424ab1385dc9337ac475752d81552a88a9b3ef37d04e"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/14
Content-Type: application/json
Authorization: Bearer dc58ac58a91ba1660c77b2c0a3910b5d9fa6aa1b41be6767a33fba646e09ea58
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
    "votable_id": 72,
    "user_id": 688
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc58ac58a91ba1660c77b2c0a3910b5d9fa6aa1b41be6767a33fba646e09ea58"
```
