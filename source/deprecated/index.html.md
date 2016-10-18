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
DELETE /v2/bookmarks/7
Content-Type: application/json
Authorization: Bearer a69478fb342d6e5a49fa7d105846d2e4bdb6b5f9ba65fdbe1ac7c1233b097420
```

`DELETE /v2/bookmarks/:bookmark_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/bookmarks/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a69478fb342d6e5a49fa7d105846d2e4bdb6b5f9ba65fdbe1ac7c1233b097420"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer e4bb5e00c480b425f340404e46540ee744c2795485936f95b3b2ff463ac834a3
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":75,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":75,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4bb5e00c480b425f340404e46540ee744c2795485936f95b3b2ff463ac834a3"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 16a0622ac83b809ed5590ef9fc75068664f335bef4dc4ce3d0575f69de2ffedb
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
    "id": 5,
    "course_id": 74,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T09:19:12.222Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:19:12.214Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":74,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16a0622ac83b809ed5590ef9fc75068664f335bef4dc4ce3d0575f69de2ffedb"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/50/bookmarks
Content-Type: application/json
Authorization: Bearer 77fe732164067117826dcdd493a6a82fd76b0c00d2b6564822e48e99a9976403
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
    "id": 5,
    "bookmarkable_id": 50,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77fe732164067117826dcdd493a6a82fd76b0c00d2b6564822e48e99a9976403"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer 39f2763679cc38d76be89a4a8dff08e9c11d76e5ff56aae81872119052515cb3
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
    "id": 1,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 27,
    "user_id": 72
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39f2763679cc38d76be89a4a8dff08e9c11d76e5ff56aae81872119052515cb3"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/74/bookmarks
Content-Type: application/json
Authorization: Bearer c70a6d514cab789e844e3ec4a19f9099d32de7c10811b8b5559400d467c4b888
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
    "bookmarkable_id": 74,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/74/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c70a6d514cab789e844e3ec4a19f9099d32de7c10811b8b5559400d467c4b888"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/53/votes
Content-Type: application/json
Authorization: Bearer dbff29bd2f878acdb82dd83efee91889543b87cd0718026b776e29386f3fbc17
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
    "votable_id": 53,
    "user_id": 186
  }
}
```



```shell
curl "api.goskive.com/v2/questions/53/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbff29bd2f878acdb82dd83efee91889543b87cd0718026b776e29386f3fbc17"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/11
Content-Type: application/json
Authorization: Bearer 5b161540069c05f02bb1232a59ee33d4e31ff61f73839b135261c17d4e51e045
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
    "votable_id": 38,
    "user_id": 123
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b161540069c05f02bb1232a59ee33d4e31ff61f73839b135261c17d4e51e045"
```
