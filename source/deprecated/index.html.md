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
DELETE /v2/bookmarks/1
Content-Type: application/json
Authorization: Bearer 2bb873730d13101506b6369d4a2f1eff98ddff04c034fb36cf28144a02817d51
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
	-H "Authorization: Bearer 2bb873730d13101506b6369d4a2f1eff98ddff04c034fb36cf28144a02817d51"
```
# Current user User Courses

## Authorisation error on create

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer cbf89ca24a3c1abdcbbbb512710f2f6c16ca8badf99c97f98dac7661a50a6db5
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":252,"pinned":true}}
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
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":252,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbf89ca24a3c1abdcbbbb512710f2f6c16ca8badf99c97f98dac7661a50a6db5"
```
## Create a user course

DEPRECATED. Use PUT /v2/courses/:course_id/pin instead.

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 39cd5f36cf8dec497d7ced86384766dcb25195c967de0e6d095ac436919e22f1
```

`POST /v2/me/user_courses`

#### Parameters


```json
{"user_course":{"course_id":253,"pinned":true}}
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
    "course_id": 253,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T13:33:23.799Z",
    "course_published": true,
    "updated_at": "2016-12-15T13:33:23.794Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -d '{"user_course":{"course_id":253,"pinned":true}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39cd5f36cf8dec497d7ced86384766dcb25195c967de0e6d095ac436919e22f1"
```
# Flashcard Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/flashcards/:flashcard_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/flashcards/95/bookmarks
Content-Type: application/json
Authorization: Bearer 9cdff7d6d79db7f4a969b503bcaf0706e851d71ba528f60c65e89c6c528c465e
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
	-H "Authorization: Bearer 9cdff7d6d79db7f4a969b503bcaf0706e851d71ba528f60c65e89c6c528c465e"
```
# Flashcard Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/flashcards/:flashcard_id/upvote PUT /v2/flashcards/:flashcard_id/downvote

### Request

#### Endpoint

```
POST /v2/flashcards/19/votes
Content-Type: application/json
Authorization: Bearer 33188dc2e4cfb42e6da5e4a403a2652140d5ec8d07d38441716985742a9ff780
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
    "id": 10,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 19,
    "user_id": 186
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/19/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33188dc2e4cfb42e6da5e4a403a2652140d5ec8d07d38441716985742a9ff780"
```
# Question Bookmarks

## Create a bookmark

DEPRECATED. Use PUT /v2/questions/:question_id/bookmark instead.

### Request

#### Endpoint

```
POST /v2/questions/126/bookmarks
Content-Type: application/json
Authorization: Bearer fe15626105d7d73b894002bef41643e5d3deeec02293205a5c2bf9fb3d573344
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
    "id": 10,
    "bookmarkable_id": 126,
    "bookmarkable_type": "Question"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/126/bookmarks" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe15626105d7d73b894002bef41643e5d3deeec02293205a5c2bf9fb3d573344"
```
# Question Votes

## Create a vote

DEPRECATED. Instead use PUT /v2/questions/:question_id/upvote PUT /v2/questions/:question_id/downvote

### Request

#### Endpoint

```
POST /v2/questions/43/votes
Content-Type: application/json
Authorization: Bearer 964a533620fb38dcbed7f1bbb101d7129e391c33ddb39ad32cc6cb65aa130cd4
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
    "id": 14,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 43,
    "user_id": 498
  }
}
```



```shell
curl "api.goskive.com/v2/questions/43/votes" -d '{"vote":{"type":"DownVote"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 964a533620fb38dcbed7f1bbb101d7129e391c33ddb39ad32cc6cb65aa130cd4"
```
# Votes

## Update a vote

DEPRECATED. Instead use PUT /v2/:content_unit_type/:content_unit_id/upvote PUT /v2/:content_unit_type/:content_unit_id/downvote

### Request

#### Endpoint

```
PATCH /v2/votes/6
Content-Type: application/json
Authorization: Bearer 3aafdd933e3d003f772c25ba2988c61d865e95e105fa690502eb22677d0bc53a
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
    "id": 6,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 14,
    "user_id": 162
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -d '{"vote":{"type":"DownVote"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aafdd933e3d003f772c25ba2988c61d865e95e105fa690502eb22677d0bc53a"
```
