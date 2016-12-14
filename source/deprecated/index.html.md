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
DELETE /v2/bookmarks/10
Content-Type: application/json
Authorization: Bearer 685dba2e08f46032036a33439809bfd95fbfb7fc1f35ffefdec3a9f239432a1c
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
	-H "Authorization: Bearer 685dba2e08f46032036a33439809bfd95fbfb7fc1f35ffefdec3a9f239432a1c"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1215ee4912da14ec85ed9ed6d65848e1418444f603f8e7ac4053c104088e3383
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":193,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":193,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1215ee4912da14ec85ed9ed6d65848e1418444f603f8e7ac4053c104088e3383"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c5a1ea6df42bfd6ae4e0799dafb66a59cfa7d53a916ff7197e24a187c7d1503e
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":192,"pinned":true}}
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
    "course_id": 192,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-14T16:47:39.258Z",
    "course_published": true,
    "updated_at": "2016-12-14T16:47:39.252Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":192,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5a1ea6df42bfd6ae4e0799dafb66a59cfa7d53a916ff7197e24a187c7d1503e"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/91/bookmarks
Content-Type: application/json
Authorization: Bearer dcc9681060ebe67d063257c506759670079cfcb0e561d03a3e32e3b8db763d32
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
    "bookmarkable_id": 91,
    "bookmarkable_type": "Flashcard"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcc9681060ebe67d063257c506759670079cfcb0e561d03a3e32e3b8db763d32"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/83/votes
Content-Type: application/json
Authorization: Bearer 20fe2630991442d61e2f7a0e63c9c0388efae7aef5c60cdd9527e9f4f913f5e7
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
    "id": 17,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 83,
    "user_id": 711
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20fe2630991442d61e2f7a0e63c9c0388efae7aef5c60cdd9527e9f4f913f5e7"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/111/bookmarks
Content-Type: application/json
Authorization: Bearer 2ee456527e31edbbdd70b558b1fc92a230f6b124e99de1ab5dab647a081429a0
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
    "bookmarkable_id": 111,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/111/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ee456527e31edbbdd70b558b1fc92a230f6b124e99de1ab5dab647a081429a0"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/74/votes
Content-Type: application/json
Authorization: Bearer 2c5ef9badcc30a7123b57d2540902106afb7db44803024e2314e546137af92be
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
    "id": 13,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 74,
    "user_id": 563
  }
}
```



```shell
curl "api.goskive.com/v2/questions/74/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c5ef9badcc30a7123b57d2540902106afb7db44803024e2314e546137af92be"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/10
Content-Type: application/json
Authorization: Bearer 8b146f7011d5d5d946829d75016a483fd46f9f2ad56ccd45b3d54ed5e7ad0118
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 48,
    "user_id": 378
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b146f7011d5d5d946829d75016a483fd46f9f2ad56ccd45b3d54ed5e7ad0118"
```
