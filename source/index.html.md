---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# Authentication

## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"25a9216a2add9f851c469a96ec0c236f42adc9c7965c59c2996af6437b12b225","client_secret":"9c4454c14485018a891170ff540bdd63fc674659c43d92449747b14fed49b336"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"25a9216a2add9f851c469a96ec0c236f42adc9c7965c59c2996af6437b12b225","client_secret":"9c4454c14485018a891170ff540bdd63fc674659c43d92449747b14fed49b336"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8e5a5ed471f9f39474aa8b7832cc90d955edb9f85314c89aa377e5bcbf164429","client_secret":"45feb6d351fde78eedab0775cefcd5be1d8e21ca03e2a9ce3c636c2b8daa53db"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8e5a5ed471f9f39474aa8b7832cc90d955edb9f85314c89aa377e5bcbf164429","client_secret":"45feb6d351fde78eedab0775cefcd5be1d8e21ca03e2a9ce3c636c2b8daa53db"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MzUwMTRiMDk0NzhjOTU5YzNhYzI0ZjY1ZWU4MzAzYzliYzMyMGY1ZDU0NmI5
ZGVjNWNkZDg5NDAyZmMwMWE3Mzo2Njg1YjM3YzBkODhmMWZiY2IzZTk2ZDYz
MWYzOTM2MmJhZTczZGRjOWYzZmY5MWQ5MGE2ZWE3YzI2YjRhZmFi

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
	-H "Content-Type: application/json" \
	-u 35014b09478c959c3ac24f65ee8303c9bc320f5d546b9dec5cdd89402fc01a73:6685b37c0d88f1fbcb3e96d631f39362bae73ddc9f3ff91d90a6ea7c26b4afab
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NzJiNjJjOGMwMmQ2NmZlNTdmYzEwMzE2NjhkZjg5ZjIwZTNlOTdjOWFhN2Ux
ZmEyYjA4Zjc0NzAwZTMxMzk0YzowMmJlMzE3YTVjOGEzMDhkZmRjYmIxNjhh
Y2M2OGQyMWExM2RhYTUzOTdhN2FiMzE2MGM3ZWJkYzMzZjQ2NzIy

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 72b62c8c02d66fe57fc1031668df89f20e3e97c9aa7e1fa2b08f74700e31394c:02be317a5c8a308dfdcbb168acc68d21a13daa5397a7ab3160c7ebdc33f46722
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"client_credentials","client_id":"1bbb7f5cdf9ba35b9966eff276e44c3c81575f8a66b753766ed17b7e24d48366","client_secret":"10fdc17c624d7be4ad4b669afa9fcebb229cfd0d268389ea558066dabb86d6aa"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| client_id *required* | Client ID |
| client_secret *required* | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "444e2777640cc34a6ed0b1ea67b0d375de60241fe0e28c5027790fb99744322b",
  "token_type": "bearer",
  "created_at": 1473336964
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"1bbb7f5cdf9ba35b9966eff276e44c3c81575f8a66b753766ed17b7e24d48366","client_secret":"10fdc17c624d7be4ad4b669afa9fcebb229cfd0d268389ea558066dabb86d6aa"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cf2320ca386a12943fe85860d36ffd865a7eefc72fa3b61b40bb74b992740590","client_secret":"7888e4e795be34ccaa43fe759c371fae1fe55f9cc55347d62b0c111047d2e6a9"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "4f2860ffb06d4c04365d67adbd4eefc8294dc99275e0bd44cff2608e70d9c758",
  "token_type": "bearer",
  "created_at": 1473336964
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cf2320ca386a12943fe85860d36ffd865a7eefc72fa3b61b40bb74b992740590","client_secret":"7888e4e795be34ccaa43fe759c371fae1fe55f9cc55347d62b0c111047d2e6a9"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NmNhMjczYTY0YjI5NDNkMGVhN2ViMjk5YjQzZDI5ZTI0OGM1M2RjODAyY2Mw
YzZkNzRiNTE0YzlhODFjNjI5ZDpmYjZjNjEyY2UxYjQzN2NhZDMyZmE3MmE1
NWM2MmYyZTZjMzZjZDkzZDAwNDc4MDlmNWMxZWUxY2VkNDg4ODBl

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "0367fbcfde3f0469a92cb761f48b000c9d63390e631bd64e10ad6a664e167240",
  "token_type": "bearer",
  "created_at": 1473336965
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 6ca273a64b2943d0ea7eb299b43d29e248c53dc802cc0c6d74b514c9a81c629d:fb6c612ce1b437cad32fa72a55c62f2e6c36cd93d0047809f5c1ee1ced48880e
```
## Validation error on create

A missing `client_id` gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "validation_failed",
      "error_description": "Validation failed: Application can't be blank"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json"
```
# Campaigns

## Get a campaign


### Request

#### Endpoint

```
GET /v2/campaigns/1
Content-Type: application/json
Authorization: Bearer df6f0756de5de099689af6daa086308f679a7b49382be1c62f1416d041d2f310
```

`GET /v2/campaigns/:campaign_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaign": {
    "id": 1,
    "title": "Recruiting pastry chefs",
    "company_id": 1,
    "precluded_campaign_ids": [

    ],
    "company_profiles": [

    ],
    "banners": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/campaigns/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df6f0756de5de099689af6daa086308f679a7b49382be1c62f1416d041d2f310"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/193/flashcards
Content-Type: application/json
Authorization: Bearer 4f31b870caa34ecfd890e509305994f1634ac602a153d52bb013817337d8929a
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":193,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 916,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:59.561Z",
    "created_at": "2016-09-08T12:16:59.561Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/193/flashcards" -d '{"flashcard":{"chapter_id":193,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f31b870caa34ecfd890e509305994f1634ac602a153d52bb013817337d8929a"
```
## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer ebc40611e76b1c37c23dcbf219f2ccebb573fe6b3d1a501c281adac26640996b
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":194,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 94,
    "obfuscated_id": "CVi6VU_nV6k",
    "author_id": 919,
    "chapter_id": 194,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:59.995Z",
    "created_at": "2016-09-08T12:16:59.995Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "",
    "back_content": "",
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/194/flashcards" -d '{"flashcard":{"chapter_id":194,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebc40611e76b1c37c23dcbf219f2ccebb573fe6b3d1a501c281adac26640996b"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/195/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 43a9394aa2f90ed5c42ae9594b84e9bc78949dc9dc8fa9a09fb6ccdf6404258c
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

195
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

fr
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 95,
    "obfuscated_id": "uTOhBSQK4CI",
    "author_id": 922,
    "chapter_id": 195,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:17:00.441Z",
    "created_at": "2016-09-08T12:17:00.441Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/7164c45e3020e9447658639b390a0409ed914be8.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/22c68308ec9f30e2692f54d80b294ee2cd9cb70c.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/7164c45e3020e9447658639b390a0409ed914be8.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/22c68308ec9f30e2692f54d80b294ee2cd9cb70c.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/195/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

195
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

fr
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X POST \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 43a9394aa2f90ed5c42ae9594b84e9bc78949dc9dc8fa9a09fb6ccdf6404258c"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/191/flashcards
Content-Type: application/json
Authorization: Bearer 402bb9565f33f6eecd02b007036d5e58f9108861b939952fecdb058f797f0083
```

`GET /v2/chapters/:chapter_id/flashcards`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcards": [
    {
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 908,
      "chapter_id": 191,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:58.903Z",
      "created_at": "2016-09-08T12:16:58.903Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 908,
      "chapter_id": 191,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:58.923Z",
      "created_at": "2016-09-08T12:16:58.923Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 908,
      "chapter_id": 191,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:58.942Z",
      "created_at": "2016-09-08T12:16:58.942Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/191/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 402bb9565f33f6eecd02b007036d5e58f9108861b939952fecdb058f797f0083"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/94/questions
Content-Type: application/json
Authorization: Bearer 77b4eec8f191b4b54fe0c43a18b0e6d879cde73b83cb56e6d079ee30b5bcf7ea
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":94,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 429,
    "chapter_id": 94,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:26.291Z",
    "created_at": "2016-09-08T12:16:26.291Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": true,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 136,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 137,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 138,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 139,
        "position": 4,
        "content": "Eggs",
        "content_html": "<p>Eggs</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/94/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":94,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77b4eec8f191b4b54fe0c43a18b0e6d879cde73b83cb56e6d079ee30b5bcf7ea"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/91/questions
Content-Type: application/json
Authorization: Bearer 9cb824c78e00b679a99d06ae2ad6b1035d5b3a546959df391fd2892e40c2444e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":91,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 65,
    "obfuscated_id": "Pu1fo5_Q1vk",
    "author_id": 420,
    "chapter_id": 91,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:25.607Z",
    "created_at": "2016-09-08T12:16:25.607Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 129,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 130,
        "position": 2,
        "content": "Flour and eggs",
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/91/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":91,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cb824c78e00b679a99d06ae2ad6b1035d5b3a546959df391fd2892e40c2444e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/92/questions
Content-Type: application/json
Authorization: Bearer 2e29f9222e00a8e88c0598e72fd5207e96fa169c2dae7cd60bf08997146b2632
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":92,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 423,
    "chapter_id": 92,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:25.833Z",
    "created_at": "2016-09-08T12:16:25.833Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": null,
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 131,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 132,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/92/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":92,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e29f9222e00a8e88c0598e72fd5207e96fa169c2dae7cd60bf08997146b2632"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/93/questions
Content-Type: application/json
Authorization: Bearer d0a3140b0c4fcd8d9de22ec6bf8916fa10773a03f8860f324ade3b8f8e0ecbc1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":93,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 67,
    "obfuscated_id": "btMCNJVyvlA",
    "author_id": 426,
    "chapter_id": 93,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:26.050Z",
    "created_at": "2016-09-08T12:16:26.050Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How many Germans does it take to change a light bulb?",
    "question_html": "How many Germans does it take to change a <strong>light bulb</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Think about German humor.",
    "explanation_html": "Think about German <strong>humor</strong>",
    "answer_options": [
      {
        "id": 133,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 134,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 135,
        "position": 3,
        "content": "Two. One that changes it and one that makes this joke work.",
        "content_html": "<p>Two. One that changes it and one that makes this joke work.</p>",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/93/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":93,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0a3140b0c4fcd8d9de22ec6bf8916fa10773a03f8860f324ade3b8f8e0ecbc1"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/96/questions
Content-Type: application/json
Authorization: Bearer 42e05532ab8600ce7cf4f03af007ff762c8c040f2e8b734407da7708c4cb70f0
```

`GET /v2/chapters/:chapter_id/questions`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "questions": [
    {
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 435,
      "chapter_id": 96,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:26.697Z",
      "created_at": "2016-09-08T12:16:26.671Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 140,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 141,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 436,
      "chapter_id": 96,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:26.764Z",
      "created_at": "2016-09-08T12:16:26.739Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 142,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 143,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 437,
      "chapter_id": 96,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-08T12:16:26.830Z",
      "created_at": "2016-09-08T12:16:26.804Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 144,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 145,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/96/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42e05532ab8600ce7cf4f03af007ff762c8c040f2e8b734407da7708c4cb70f0"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/82
Content-Type: application/json
Authorization: Bearer db3c6d3ab2b74b5ad4ef0374837195fdd3f1a70ebe51be1369e3c13704ee7dca
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


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
curl "api.goskive.com/v2/chapters/82" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db3c6d3ab2b74b5ad4ef0374837195fdd3f1a70ebe51be1369e3c13704ee7dca"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/84
Content-Type: application/json
Authorization: Bearer e1a3ef69c3fc0ece75b3c409a18c30f78b3017c4dadf7ae4098d0f8f927eb19a
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


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
curl "api.goskive.com/v2/chapters/84" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1a3ef69c3fc0ece75b3c409a18c30f78b3017c4dadf7ae4098d0f8f927eb19a"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/80
Content-Type: application/json
Authorization: Bearer c810d3ae141b8bf2cfd8a2a970d62a68ed26de926706d2b7dc848501e4c97d01
```

`PATCH /v2/chapters/:chapter_id`

#### Parameters


```json
{"chapter":{"title":"Eggs and Flour"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title]  | Chapter title |
| chapter[position]  | Position |



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
curl "api.goskive.com/v2/chapters/80" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c810d3ae141b8bf2cfd8a2a970d62a68ed26de926706d2b7dc848501e4c97d01"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/83
Content-Type: application/json
Authorization: Bearer 1d1d1383d05a559006c8657953493e48ce03405ae76252d1ccd305bf5e89a07d
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/83" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d1d1383d05a559006c8657953493e48ce03405ae76252d1ccd305bf5e89a07d"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/77
Content-Type: application/json
Authorization: Bearer ff3561648acde97d8bb10a2ab7f92cd08b898c6d337a8acf60b5fcee0e244b4d
```

`GET /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapter": {
    "id": 77,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-08T12:16:22.551Z",
    "course_id": 133,
    "author_id": 366,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 370,
        "chapter_id": 77,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-09-08T12:16:22.546Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      }
    ],
    "questions": [
      {
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 368,
        "chapter_id": 77,
        "position": 59,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-09-08T12:16:22.444Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 117,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 118,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/77" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff3561648acde97d8bb10a2ab7f92cd08b898c6d337a8acf60b5fcee0e244b4d"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/78
Content-Type: application/json
Authorization: Bearer da79117a351c059ba7487fdda9ce4fb7ba946f48ce58cadd3fd5ef5dc7148a1c
```

`PATCH /v2/chapters/:chapter_id`

#### Parameters


```json
{"chapter":{"title":"Eggs and Flour"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title]  | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapter": {
    "id": 78,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-08T12:16:22.755Z",
    "course_id": 134,
    "author_id": 373,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": null,
    "questions_updated_at": null,
    "flashcards_count": 0,
    "questions_count": 0,
    "flashcards": [

    ],
    "questions": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/78" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da79117a351c059ba7487fdda9ce4fb7ba946f48ce58cadd3fd5ef5dc7148a1c"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/59/replies
Content-Type: application/json
Authorization: Bearer dd80049d7cae2f5e0a0a628d1c4d771ad0fcb1484398c5c467b99cfce59fe0f1
```

`POST /v2/comments/:comment_id/replies`

#### Parameters


```json
{"comment":{"message":"Just keeping the thread alive!"}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 60,
    "author_id": 820,
    "reply_to_id": 59,
    "created_at": "2016-09-08T12:16:52.623Z",
    "status": "published",
    "message": "Just keeping the thread alive!",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |


```shell
curl "api.goskive.com/v2/comments/59/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd80049d7cae2f5e0a0a628d1c4d771ad0fcb1484398c5c467b99cfce59fe0f1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer c3e188df1371b4b788f372672c599d45ce90ff41031b65104ec231977eb44c75
```

`POST /v2/comments/:comment_id/replies`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |


```shell
curl "api.goskive.com/v2/comments/58/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3e188df1371b4b788f372672c599d45ce90ff41031b65104ec231977eb44c75"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer 0aa961c5a840a473a105c9acb7312b598f022e81cfe96d2a17663e624cf2111f
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


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
curl "api.goskive.com/v2/comments/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aa961c5a840a473a105c9acb7312b598f022e81cfe96d2a17663e624cf2111f"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/51/republish
Content-Type: application/json
Authorization: Bearer 02886e9990e7457a89db6cc35f7cd3cea1733f486508e88295cff5cac5d90e73
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


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
curl "api.goskive.com/v2/comments/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02886e9990e7457a89db6cc35f7cd3cea1733f486508e88295cff5cac5d90e73"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer aea6b82821b953a7e4354cb8e20de96c7995aef30aedf97a4260030c8d23482e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aea6b82821b953a7e4354cb8e20de96c7995aef30aedf97a4260030c8d23482e"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/52/report
Content-Type: application/json
Authorization: Bearer 4665e0d9aa091f8a8ee2c04b1f58407f72166d6dd2136593fe245ffb7b1b9ed3
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4665e0d9aa091f8a8ee2c04b1f58407f72166d6dd2136593fe245ffb7b1b9ed3"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/11
Content-Type: application/json
Authorization: Bearer edfe163e493d0ca425ea1d0e0bc3dffe5fea4b6c88fd048b35f5493b129dc3b9
```

`GET /v2/companies/:company_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company": {
    "id": 11,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-09-08T12:16:06.905Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edfe163e493d0ca425ea1d0e0bc3dffe5fea4b6c88fd048b35f5493b129dc3b9"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 315b6ab4208484b4638d94be189a8a1d6df2d16e93ccb2cf0bbf037877cf536e
```

`GET /v2/companies`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "companies": [
    {
      "id": 8,
      "name": "Fake Company Name 7",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-08T12:16:06.839Z"
    },
    {
      "id": 9,
      "name": "Fake Company Name 8",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-08T12:16:06.844Z"
    },
    {
      "id": 10,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-08T12:16:06.848Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 315b6ab4208484b4638d94be189a8a1d6df2d16e93ccb2cf0bbf037877cf536e"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer ecd9af7726fd7548e59c56b1a304ce7ff2cd05100095cedd8db014c23e3ddad3
```

`GET /v2/companies/:company_id/company_profiles`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company_profiles": [
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 9,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/87f24f1d1c22af87a4c49901ca6db1d9205da6e7.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/c88539f34738a470d3868a5d08c1e5a58443cdb0.png",
      "widgets": [

      ]
    },
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 8,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/4e8ccb4fdbb03332710724b7199bfb925ebb8588.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/1751c1fcb04de04c20e97d74547e239755abd978.png",
      "widgets": [

      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecd9af7726fd7548e59c56b1a304ce7ff2cd05100095cedd8db014c23e3ddad3"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/24/company_profiles
Content-Type: application/json
Authorization: Bearer 1e83b8d809d2e6e8ef54e6d8a2bc8295bb62257e1ef0faa78459bd9990b099c6
```

`GET /v2/companies/:company_id/company_profiles`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company_profiles": [
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 5,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/43cd8331a2a1101475dca8b52baf14565bda8d25.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/36ab23184d8eb9448413fbe09f112b2034c6db2d.png",
      "widgets": [
        {
          "id": 1,
          "type": "twitter",
          "prompt": "Check us out on Twitter",
          "username": "SkiveApp",
          "fallback_url": "https://goskive.com"
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/24/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e83b8d809d2e6e8ef54e6d8a2bc8295bb62257e1ef0faa78459bd9990b099c6"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer f9084e0b05f2f928ec70489f1636ac0326d270f549e7d45244f54a347b8f7672
```

`GET /v2/courses/:course_slug/campaigns`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaigns": [
    {
      "id": 2,
      "title": "Campaign 1",
      "company_id": 12,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 1,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/0adf1955ecfb39ff0d02f85dd384e7aeaf694927.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/39195f7a12fa003c1584dcee68597ed4a180cb4b.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/8dbf7d28f3cbdc6d654d6324af20a11fe3653b85.png",
          "target_url": "http://goskive.com",
          "id": 1,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 5,
      "title": "Campaign 4",
      "company_id": 15,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 2,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9eceef98bbb4cbbf925777c91787755d8353de98.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/a56a082a30d2de9bc36364cd610c75501bd3b7d5.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/889019b341716d48f4f28718872d4f688cd18499.png",
          "target_url": "http://goskive.com",
          "id": 2,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9084e0b05f2f928ec70489f1636ac0326d270f549e7d45244f54a347b8f7672"
```
# Course Chapters

## Authorisation error on create

A student may not create a chapter in an unpublished
            course.

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e06dbe86edaaba7d4180eed7438107b01158e89a9cff8095005a2f3f4a9614b4
```

`POST /v2/courses/:course_slug/chapters`

#### Parameters


```json
{"chapter":{"title":"Preparing the oven"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title] *required* | Chapter title |
| chapter[position]  | Position |



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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e06dbe86edaaba7d4180eed7438107b01158e89a9cff8095005a2f3f4a9614b4"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d2ee2802bb4f4463ae424cfb19c25b095a647812d395b305cf4ee2772d221913
```

`POST /v2/courses/:course_slug/chapters`

#### Parameters


```json
{"chapter":{"title":"Preparing the oven"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title] *required* | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "chapter": {
    "id": 141,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-08T12:16:49.915Z",
    "course_id": 254,
    "author_id": 764,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": null,
    "questions_updated_at": null,
    "flashcards_count": 0,
    "questions_count": 0,
    "flashcards": [

    ],
    "questions": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2ee2802bb4f4463ae424cfb19c25b095a647812d395b305cf4ee2772d221913"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6429c42b8e3c6bb5367cbc7ed53f26479e1046bc4c11414deadcc8dfa4cb842e
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 145,
      "title": "Clever Chapter Title 124",
      "position": 1,
      "updated_at": "2016-09-08T12:16:50.408Z",
      "course_id": 257,
      "author_id": 773,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 146,
      "title": "Clever Chapter Title 125",
      "position": 2,
      "updated_at": "2016-09-08T12:16:50.431Z",
      "course_id": 257,
      "author_id": 774,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 147,
      "title": "Clever Chapter Title 126",
      "position": 3,
      "updated_at": "2016-09-08T12:16:50.555Z",
      "course_id": 257,
      "author_id": 775,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-09-08T12:16:50.545Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6429c42b8e3c6bb5367cbc7ed53f26479e1046bc4c11414deadcc8dfa4cb842e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 151,
      "title": "Clever Chapter Title 130",
      "position": 1,
      "updated_at": "2016-09-08T12:16:51.068Z",
      "course_id": 260,
      "author_id": 787,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 152,
      "title": "Clever Chapter Title 131",
      "position": 2,
      "updated_at": "2016-09-08T12:16:51.091Z",
      "course_id": 260,
      "author_id": 788,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 153,
      "title": "Clever Chapter Title 132",
      "position": 3,
      "updated_at": "2016-09-08T12:16:51.213Z",
      "course_id": 260,
      "author_id": 789,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-09-08T12:16:51.203Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 14ca3113cbdb9b2ae6528867599445d2a4cac0bfefcf42dd3f15f945252bd227
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 148,
      "title": "Clever Chapter Title 127",
      "position": 1,
      "updated_at": "2016-09-08T12:16:50.840Z",
      "course_id": 259,
      "author_id": 782,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 149,
      "title": "Clever Chapter Title 128",
      "position": 2,
      "updated_at": "2016-09-08T12:16:50.865Z",
      "course_id": 259,
      "author_id": 783,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 150,
      "title": "Clever Chapter Title 129",
      "position": 3,
      "updated_at": "2016-09-08T12:16:50.890Z",
      "course_id": 259,
      "author_id": 784,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14ca3113cbdb9b2ae6528867599445d2a4cac0bfefcf42dd3f15f945252bd227"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 154,
      "title": "Clever Chapter Title 133",
      "position": 1,
      "updated_at": "2016-09-08T12:16:51.340Z",
      "course_id": 261,
      "author_id": 793,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 155,
      "title": "Clever Chapter Title 134",
      "position": 2,
      "updated_at": "2016-09-08T12:16:51.364Z",
      "course_id": 261,
      "author_id": 794,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 156,
      "title": "Clever Chapter Title 135",
      "position": 3,
      "updated_at": "2016-09-08T12:16:51.389Z",
      "course_id": 261,
      "author_id": 795,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f4cfdea6147f2bb5a2273bf6af130e95518fb82f5a7ca587c27e5d4db94b5d81
```

`POST /v2/courses/:course_slug/course_requests`

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
  "course_request": {
    "id": 3,
    "course_id": 190,
    "user_id": 600,
    "updated_at": "2016-09-08T12:16:41.357Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4cfdea6147f2bb5a2273bf6af130e95518fb82f5a7ca587c27e5d4db94b5d81"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 43203d920cf456afbde6eb05033f0d8138232617f5b40a83c9bcaa8b9dfdc8e5
```

`GET /v2/courses/:course_slug/course_requests`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course_requests": [
    {
      "id": 6,
      "course_id": 194,
      "user_id": 610,
      "updated_at": "2016-09-08T12:16:41.937Z"
    },
    {
      "id": 7,
      "course_id": 194,
      "user_id": 611,
      "updated_at": "2016-09-08T12:16:41.954Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43203d920cf456afbde6eb05033f0d8138232617f5b40a83c9bcaa8b9dfdc8e5"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 1b921cce2e11a0eb793b94d5cd3fc57a99934a3297047a98ef9619aa97e3c5c2
```

`DELETE /v2/course_requests/:course_request_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/course_requests/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b921cce2e11a0eb793b94d5cd3fc57a99934a3297047a98ef9619aa97e3c5c2"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e1c94f487384ac57213ba27b94d83998bac1ca611bf691a00036e8fd65544f7d
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1c94f487384ac57213ba27b94d83998bac1ca611bf691a00036e8fd65544f7d"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e9fd7653476378dbff4e7260e8f3b3cc58e2cb9467d9d97bcffc700cafcdde10
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9fd7653476378dbff4e7260e8f3b3cc58e2cb9467d9d97bcffc700cafcdde10"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 81f3bae84dcac92f22c4f05e5c8c4f0c96f984d1f4a265e763e1e192601e62d9
```

`PATCH /v2/courses/:course_slug`

#### Parameters


```json
{"course":{"title":"Choux pastry 102","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| course[title]  | Title |
| course[topic_id]  | Topic ID |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |



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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81f3bae84dcac92f22c4f05e5c8c4f0c96f984d1f4a265e763e1e192601e62d9"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b9b7f179c4007a35d39e22c788eff809fcdc0aba412225d5f75ddc9edd10a0a5
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9b7f179c4007a35d39e22c788eff809fcdc0aba412225d5f75ddc9edd10a0a5"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug`

#### Parameters


```json
include: questions
```


| Name | Description |
|:-----|:------------|
| include  | optional resources to embed |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 256,
    "id": 72,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 77,
    "additional_university_ids": [

    ],
    "topic_id": 79,
    "discipline_id": 80,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 2,
    "questions_count": 2,
    "users_count": 0,
    "user_generated": false,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": true,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-08T12:16:13.229Z",
    "updated_at": "2016-09-08T12:16:13.231Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 57,
        "title": "Clever Chapter Title 57",
        "position": 1,
        "updated_at": "2016-09-08T12:16:13.200Z",
        "course_id": 72,
        "author_id": 256,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-08T12:16:13.098Z",
        "questions_updated_at": "2016-09-08T12:16:12.759Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 58,
        "title": "Clever Chapter Title 58",
        "position": 2,
        "updated_at": "2016-09-08T12:16:13.229Z",
        "course_id": 72,
        "author_id": 256,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-08T12:16:13.143Z",
        "questions_updated_at": "2016-09-08T12:16:12.879Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 256,
        "chapter_id": 57,
        "position": 26,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:12.759Z",
        "created_at": "2016-09-08T12:16:12.733Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 256,
        "chapter_id": 58,
        "position": 28,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:12.879Z",
        "created_at": "2016-09-08T12:16:12.854Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 55,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 56,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer d3153b3d9e2013fee29deb1b548890141ce9dcdd047f3f1538b3c4ba8d735bec
```

`GET /v2/courses/:course_slug`

#### Parameters


```json
include: questions, flashcards
```


| Name | Description |
|:-----|:------------|
| include  | optional resources to embed |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 267,
    "id": 74,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 79,
    "additional_university_ids": [

    ],
    "topic_id": 81,
    "discipline_id": 82,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 4,
    "questions_count": 4,
    "users_count": 0,
    "user_generated": false,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": true,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-08T12:16:14.612Z",
    "updated_at": "2016-09-08T12:16:14.614Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 61,
        "title": "Clever Chapter Title 61",
        "position": 1,
        "updated_at": "2016-09-08T12:16:14.584Z",
        "course_id": 74,
        "author_id": 267,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-08T12:16:14.510Z",
        "questions_updated_at": "2016-09-08T12:16:14.181Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 62,
        "title": "Clever Chapter Title 62",
        "position": 2,
        "updated_at": "2016-09-08T12:16:14.612Z",
        "course_id": 74,
        "author_id": 267,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-08T12:16:14.551Z",
        "questions_updated_at": "2016-09-08T12:16:14.307Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 268,
        "chapter_id": 61,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.487Z",
        "created_at": "2016-09-08T12:16:14.487Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 268,
        "chapter_id": 62,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.529Z",
        "created_at": "2016-09-08T12:16:14.529Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 268,
        "chapter_id": 61,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.510Z",
        "created_at": "2016-09-08T12:16:14.510Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 268,
        "chapter_id": 62,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.551Z",
        "created_at": "2016-09-08T12:16:14.551Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      }
    ],
    "questions": [
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 268,
        "chapter_id": 61,
        "position": 38,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.126Z",
        "created_at": "2016-09-08T12:16:14.101Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 75,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 76,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 268,
        "chapter_id": 61,
        "position": 39,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.181Z",
        "created_at": "2016-09-08T12:16:14.157Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 77,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 78,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 268,
        "chapter_id": 62,
        "position": 40,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.248Z",
        "created_at": "2016-09-08T12:16:14.223Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 79,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 80,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 268,
        "chapter_id": 62,
        "position": 41,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-08T12:16:14.307Z",
        "created_at": "2016-09-08T12:16:14.281Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 81,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 82,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3153b3d9e2013fee29deb1b548890141ce9dcdd047f3f1538b3c4ba8d735bec"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/76/pin
Content-Type: application/json
Authorization: Bearer f8194a849d693fffb31583122dd0b989312dc2eb6e23ec873efb1de89a86714c
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/76/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8194a849d693fffb31583122dd0b989312dc2eb6e23ec873efb1de89a86714c"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/71/pin
Content-Type: application/json
Authorization: Bearer 19af3cbcee2f3252bd85e9ac2daecf6db1767745e7ee9e3222d2408720cb8264
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/71/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19af3cbcee2f3252bd85e9ac2daecf6db1767745e7ee9e3222d2408720cb8264"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ba1fb528372e507a6ccb43e2c9dec1b4fb1c9b74e5437aa1427a6efcac5c9fa2
```

`PATCH /v2/courses/:course_slug`

#### Parameters


```json
{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}
```


| Name | Description |
|:-----|:------------|
| course[title]  | Title |
| course[topic_id]  | Topic ID |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 249,
    "id": 68,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 73,
    "additional_university_ids": [

    ],
    "topic_id": 75,
    "discipline_id": 76,
    "language_code": "fr",
    "exam_months": [

    ],
    "title": "Choux pastry 102",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-09-08T12:16:12.163Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba1fb528372e507a6ccb43e2c9dec1b4fb1c9b74e5437aa1427a6efcac5c9fa2"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer bf55fc187fd507c1c37e9a9553c263f8373352757e6e2b8361b0277dac5c6474
```

`GET /v2/me/user`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 115,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:02.032Z",
    "updated_at": "2016-09-08T12:16:02.032Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf55fc187fd507c1c37e9a9553c263f8373352757e6e2b8361b0277dac5c6474"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a3dba30dd11f626af54315b25bc1f18bc7ebc8c4016db9265ffd9f55e3034c74
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[36]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 117,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      36
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:02.421Z",
    "updated_at": "2016-09-08T12:16:02.459Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[36]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3dba30dd11f626af54315b25bc1f18bc7ebc8c4016db9265ffd9f55e3034c74"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 54c1745f0ff1a38d79b362c5cb366a6f98bb6bc8628a4aa262542f18bae218fb
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 119,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:02.561Z",
    "updated_at": "2016-09-08T12:16:02.561Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54c1745f0ff1a38d79b362c5cb366a6f98bb6bc8628a4aa262542f18bae218fb"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1dc36db4863908db3e6a2de050c2b1b4a4d90a24f91937b346c2312a86da47f5
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[39]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 120,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      39
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:02.662Z",
    "updated_at": "2016-09-08T12:16:02.662Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[39]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1dc36db4863908db3e6a2de050c2b1b4a4d90a24f91937b346c2312a86da47f5"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 906df6984833438351330d0fdb785443b8c4432d1b42bbea6586e9ff76d69eaa
```

`PATCH /v2/me/user`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="email"

magnus@gmail.sk
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="first_name"

Sven
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="fields_of_study[]"

35
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 116,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/faf0df07b2db0534e63019fba9970f44944dcfa8.jpg",
    "university_id": null,
    "fields_of_study": [
      35
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:02.137Z",
    "updated_at": "2016-09-08T12:16:02.368Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/3d8d03545b1b0949be1fc9ef03db36277b7c406c.jpg",
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="email"

magnus@gmail.sk
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="first_name"

Sven
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="fields_of_study[]"

35
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 906df6984833438351330d0fdb785443b8c4432d1b42bbea6586e9ff76d69eaa"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer fde700751d52ef04d3279f86e1940be92ef36ed343913b769f76410be65ad3d8
```

`GET /v2/me/bookmarks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "bookmarks": [
    {
      "id": 4,
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fde700751d52ef04d3279f86e1940be92ef36ed343913b769f76410be65ad3d8"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1c08d5208eb1b51ada193cdbbc6b6e32ca0b27e1006b6abd0267659823257093
```

`GET /v2/me/campaigns`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaigns": [
    {
      "id": 10,
      "title": "Campaign 9",
      "company_id": 27,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 10,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/653938ceeed87e42b62d7feeca02cd82da1acb27.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/d204067fe9ed5e993ed4b1188ce57016fdd8b991.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/498551b0a405b9134839281bc158747e85383832.png",
          "target_url": "http://goskive.com",
          "id": 5,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 11,
      "title": "Campaign 10",
      "company_id": 28,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 11,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/6557160cf523e6b44ee9eac06061463b0fcbd3b1.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/f4961300e395cd3802066da84ade8e1cdd20826f.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/8aa5bf11cc13a7de5c7089d33a8ff916dd8f8472.png",
          "target_url": "http://goskive.com",
          "id": 6,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c08d5208eb1b51ada193cdbbc6b6e32ca0b27e1006b6abd0267659823257093"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer fc6fc7187d3bfe1a5c14469fb3986ffed2bdcf0db84c66a09a4a4906cc4610a9
```

`GET /v2/me/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 355,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-103",
      "html_url": "https://goskive.com/course/mit-course-103",
      "slug": "mit-course-103",
      "university_id": 114,
      "additional_university_ids": [

      ],
      "topic_id": 137,
      "discipline_id": 138,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:21.623Z",
      "shortname": "mit-course-103"
    },
    {
      "creator_id": 356,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-104",
      "html_url": "https://goskive.com/course/mit-course-104",
      "slug": "mit-course-104",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 138,
      "discipline_id": 139,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:21.707Z",
      "shortname": "mit-course-104"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc6fc7187d3bfe1a5c14469fb3986ffed2bdcf0db84c66a09a4a4906cc4610a9"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 27d03c64517dbcbe1d00f7be4e7d82626d65a7d2e51cc2504d21d01bce2a13c3
```

`GET /v2/me/jobs`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "job_postings": [
    {
      "id": 1,
      "title": "Job Posting1",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 2,
      "company": {
        "id": 2,
        "name": "Fake Company Name 1",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
        "brand_color": "#000000",
        "updated_at": "2016-09-08T12:16:01.453Z"
      },
      "created_at": "2016-09-08T12:16:01.458Z",
      "updated_at": "2016-09-08T12:16:01.458Z"
    },
    {
      "id": 1,
      "title": "Job Posting1",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 2,
      "company": {
        "id": 2,
        "name": "Fake Company Name 1",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
        "brand_color": "#000000",
        "updated_at": "2016-09-08T12:16:01.453Z"
      },
      "created_at": "2016-09-08T12:16:01.458Z",
      "updated_at": "2016-09-08T12:16:01.458Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27d03c64517dbcbe1d00f7be4e7d82626d65a7d2e51cc2504d21d01bce2a13c3"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 4e318302418ee1bc84d3f31b40a9d59aa2fd4d5793623099b69b4cc9c68344e2
```

`GET /v2/me/notifications`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "notifications": [
    {
      "type": "CommentNotification",
      "id": 10,
      "created_at": "2016-09-08T12:16:09.599Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 11,
      "updated_at": "2016-09-08T12:16:09.716Z",
      "author_id": "209",
      "thread_subject_id": "54",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 11,
      "created_at": "2016-09-08T12:16:09.702Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 12,
      "updated_at": "2016-09-08T12:16:09.719Z",
      "author_id": "212",
      "thread_subject_id": "55",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 12,
      "created_at": "2016-09-08T12:16:09.902Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-09-08T12:16:09.902Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-09-08T12:16:10.082Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-09-08T12:16:10.082Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 14,
      "created_at": "2016-09-08T12:16:10.268Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-09-08T12:16:10.268Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 15,
      "created_at": "2016-09-08T12:16:10.423Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 23,
      "updated_at": "2016-09-08T12:16:10.423Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 16,
      "created_at": "2016-09-08T12:16:10.584Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 24,
      "updated_at": "2016-09-08T12:16:10.584Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-09-08T12:16:10.739Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 25,
      "updated_at": "2016-09-08T12:16:10.739Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e318302418ee1bc84d3f31b40a9d59aa2fd4d5793623099b69b4cc9c68344e2"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/18
Content-Type: application/json
Authorization: Bearer 73fed821ed4103303b8a601a0d417c2827ba322a26c286d6075c14e5d7c973bd
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-09-08T12:06:10.000Z"}}
```


| Name | Description |
|:-----|:------------|
| notification[read_at]  | Read at |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "notification": {
    "type": "CommentNotification",
    "id": 18,
    "created_at": "2016-09-08T12:16:10.885Z",
    "read_at": "2016-09-08T12:06:10.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 13,
    "updated_at": "2016-09-08T12:16:10.927Z",
    "author_id": "237",
    "thread_subject_id": "62",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/18" -d '{"notification":{"read_at":"2016-09-08T12:06:10.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73fed821ed4103303b8a601a0d417c2827ba322a26c286d6075c14e5d7c973bd"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 78c2987f6ec78c825214586ff9b72785e445878044c9bf04d213a00c6dffeb02
```

`GET /v2/me/user_courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_courses": [
    {
      "id": 10,
      "course_id": 239,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-08T12:16:47.239Z",
      "course_published": true,
      "updated_at": "2016-09-08T12:16:47.230Z"
    },
    {
      "id": 11,
      "course_id": 240,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-08T12:16:47.329Z",
      "course_published": true,
      "updated_at": "2016-09-08T12:16:47.320Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78c2987f6ec78c825214586ff9b72785e445878044c9bf04d213a00c6dffeb02"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer fc004fd91900337c68892fe5a3aecd7b9c15692a1e7bb707b80a82c35b7e9ffb
```

`GET /v2/me/user_courses/:user_course_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_course": {
    "id": 8,
    "course_id": 237,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-08T12:16:46.942Z",
    "course_published": true,
    "updated_at": "2016-09-08T12:16:46.933Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc004fd91900337c68892fe5a3aecd7b9c15692a1e7bb707b80a82c35b7e9ffb"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/9
Content-Type: application/json
Authorization: Bearer 2f5e120538f7bc9721011fb8dd0b4523d169ca7f236576a444fd89bad1d53cd7
```

`PATCH /v2/me/user_courses/:user_course_id`

#### Parameters


```json
{"user_course":{"pinned":false}}
```


| Name | Description |
|:-----|:------------|
| user_course[course_id]  | Course ID |
| user_course[pinned]  | Pinned |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_course": {
    "id": 9,
    "course_id": 238,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-09-08T12:16:47.131Z",
    "course_published": true,
    "updated_at": "2016-09-08T12:16:47.124Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/9" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f5e120538f7bc9721011fb8dd0b4523d169ca7f236576a444fd89bad1d53cd7"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 2a411692285b96c6db367cea971cc3ec2832449e5f4f4fcec76308f47d468f35
```

`GET /v2/me/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 94
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 3,
      "user_id": 94
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 4,
      "user_id": 94
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 5,
      "user_id": 94
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a411692285b96c6db367cea971cc3ec2832449e5f4f4fcec76308f47d468f35"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/51
Content-Type: application/json
```

`GET /v2/disciplines/:discipline_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "discipline": {
    "id": 51,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 49,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 51
      },
      {
        "id": 50,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 51
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/51" -X GET \
	-H "Content-Type: application/json"
```
## Get a list of disciplines


### Request

#### Endpoint

```
GET /v2/disciplines
Content-Type: application/json
```

`GET /v2/disciplines`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "disciplines": [
    {
      "id": 49,
      "name": "Programmable clear-thinking forecast",
      "name_translations": {
        "en": "Programmable clear-thinking forecast"
      }
    },
    {
      "id": 50,
      "name": "Centralized coherent Graphical User Interface",
      "name_translations": {
        "en": "Centralized coherent Graphical User Interface"
      }
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/disciplines" -X GET \
	-H "Content-Type: application/json"
```
# Feedback

## Change feedback state to &#39;closed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/close
Content-Type: application/json
Authorization: Bearer 943f3078821f186c01b6e8cc7ea5193a402a7917a2235cdbc5f6bc1a9f418d96
```

`PATCH /v2/feedbacks/:feedback_id/close`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 13,
    "user_id": 454,
    "feedbackable_id": 71,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-09-08T12:16:27.549Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/13/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 943f3078821f186c01b6e8cc7ea5193a402a7917a2235cdbc5f6bc1a9f418d96"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/17/fix
Content-Type: application/json
Authorization: Bearer c3992d2cffe82bd8737ac6d1975fb2d70651a3d237b5d2ad1aced729fdbe16b7
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 17,
    "user_id": 474,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-09-08T12:16:28.536Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/17/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3992d2cffe82bd8737ac6d1975fb2d70651a3d237b5d2ad1aced729fdbe16b7"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/11
Content-Type: application/json
Authorization: Bearer 5585ec12a39f67ff28acec74e29370c6f0f2896cf243613acb88f4f1ba7a26bf
```

`GET /v2/feedbacks/:feedback_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 11,
    "user_id": 442,
    "feedbackable_id": 69,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-08T12:16:27.081Z",
    "flags": 2,
    "message": ""
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |
| feedback[message] | Message (of comment) |


```shell
curl "api.goskive.com/v2/feedbacks/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5585ec12a39f67ff28acec74e29370c6f0f2896cf243613acb88f4f1ba7a26bf"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/15/close
Content-Type: application/json
Authorization: Bearer 8722ddaccaa8c1bd103fe93337377bb3f3381c29dc951d2c02a6402637472a04
```

`PATCH /v2/feedbacks/:feedback_id/close`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "There is no event close defined for the closed state"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/15/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8722ddaccaa8c1bd103fe93337377bb3f3381c29dc951d2c02a6402637472a04"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/fix
Content-Type: application/json
Authorization: Bearer 485aaf3e4956c8456897997357b526d1c2ef140470291a12c688e81a39470ad3
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "There is no event fix defined for the closed state"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/16/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 485aaf3e4956c8456897997357b526d1c2ef140470291a12c688e81a39470ad3"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/fix
Content-Type: application/json
Authorization: Bearer 74c25aa035d7182b04c6ba5d368d6729af727f4f075765381d91128f3f4905d9
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "Content Unit was not corrected"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/19/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74c25aa035d7182b04c6ba5d368d6729af727f4f075765381d91128f3f4905d9"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/12
Content-Type: application/json
Authorization: Bearer 49753dabe1f9b67979e74f961f83ac90f574375e4668b99f10b11e89b8bcc07f
```

`GET /v2/feedbacks/:feedback_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 12,
    "user_id": 447,
    "feedbackable_id": 70,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-08T12:16:27.369Z",
    "flags": 0,
    "message": "Pi equals 2"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |
| feedback[message] | Message (of comment) |


```shell
curl "api.goskive.com/v2/feedbacks/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49753dabe1f9b67979e74f961f83ac90f574375e4668b99f10b11e89b8bcc07f"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/29/comments
Content-Type: application/json
Authorization: Bearer 93a5efbf3d8232885d2ddd7accc9ea009ed702a7814ff5894fc4dfb0d973a652
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{"comment":{"message":"This flashcard is particularly helpful!"}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 4,
    "author_id": 178,
    "reply_to_id": null,
    "created_at": "2016-09-08T12:16:07.650Z",
    "status": "published",
    "replies": [

    ],
    "message": "This flashcard is particularly helpful!",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/29/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93a5efbf3d8232885d2ddd7accc9ea009ed702a7814ff5894fc4dfb0d973a652"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/27/comments
Content-Type: application/json
Authorization: Bearer 7890463bbcd5add2a4482760b19894e527493f61a82ea557033545014ee2eaee
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 3,
    "author_id": 172,
    "reply_to_id": null,
    "created_at": "2016-09-08T12:16:07.182Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 172,
      "feedbackable_id": 27,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:07.178Z",
      "flags": 3,
      "message": "Hard to see the formulae."
    }
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/27/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7890463bbcd5add2a4482760b19894e527493f61a82ea557033545014ee2eaee"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/30/comments
Content-Type: application/json
Authorization: Bearer b713164763f9f684682a135adc8554698c430d10a4185d2944407a945909e209
```

`GET /v2/flashcards/:flashcard_id/comments`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 5,
      "author_id": 184,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:07.929Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 185,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:07.947Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/30/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b713164763f9f684682a135adc8554698c430d10a4185d2944407a945909e209"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/28/comments
Content-Type: application/json
Authorization: Bearer f306f81b02afd1f04524afa0c3235f4a30df37b25ff134d36c052befb7efaee5
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank",
      "is too short (minimum is 2 characters)"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/28/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f306f81b02afd1f04524afa0c3235f4a30df37b25ff134d36c052befb7efaee5"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/feedbacks
Content-Type: application/json
Authorization: Bearer 08c048b6fbfe05b5efe932701c66fda65347476f905c2054c2ebc6554d4ca9fe
```

`POST /v2/flashcards/:flashcard_id/feedbacks`

#### Parameters


```json
{"feedback":{"message":"No comprendo","flags":0}}
```


| Name | Description |
|:-----|:------------|
| feedback[message]  | Comment message |
| feedback[flags]  | Feedback flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "feedback": {
    "id": 46,
    "user_id": 754,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-08T12:16:49.253Z",
    "flags": 0,
    "message": "No comprendo"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/85/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08c048b6fbfe05b5efe932701c66fda65347476f905c2054c2ebc6554d4ca9fe"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/78/feedbacks
Content-Type: application/json
Authorization: Bearer d02ee66c07c12b63ccff25b687016fe6c64ff4c93a6ffcd789fdbb96b1f4acc8
```

`GET /v2/flashcards/:flashcard_id/feedbacks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedbacks": [
    {
      "id": 40,
      "user_id": 725,
      "feedbackable_id": 78,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:47.792Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 724,
      "feedbackable_id": 78,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:47.778Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/78/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d02ee66c07c12b63ccff25b687016fe6c64ff4c93a6ffcd789fdbb96b1f4acc8"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/68/votes
Content-Type: application/json
Authorization: Bearer 5905100d3d0dad43b3e0cfb14903a5947b3d0f14cef116db48d4fcbc0c0a8808
```

`GET /v2/flashcards/:flashcard_id/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 417
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 416
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 415
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/68/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5905100d3d0dad43b3e0cfb14903a5947b3d0f14cef116db48d4fcbc0c0a8808"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/18/republish
Content-Type: application/json
Authorization: Bearer 02fe4e1aa6851e679a09e17ee9fc7bdf3c690c104a63e16cc4b0dae75fc3210a
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


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
curl "api.goskive.com/v2/flashcards/18/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02fe4e1aa6851e679a09e17ee9fc7bdf3c690c104a63e16cc4b0dae75fc3210a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/19/bookmark
Content-Type: application/json
Authorization: Bearer 0e2187a2df4f372d0659059624fce49f6fc77e5b54ac0bb294eeb89f23d6402e
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e2187a2df4f372d0659059624fce49f6fc77e5b54ac0bb294eeb89f23d6402e"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/21
Content-Type: application/json
Authorization: Bearer e74a021c90bd1b75807715c5887880ab28711d00ec5fd5fa27832f2927379772
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e74a021c90bd1b75807715c5887880ab28711d00ec5fd5fa27832f2927379772"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/downvote
Content-Type: application/json
Authorization: Bearer 61de2c724cac48c453cf64b5f030fffcf4f9d9e994b3f0e47e0ad4437905b5b9
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61de2c724cac48c453cf64b5f030fffcf4f9d9e994b3f0e47e0ad4437905b5b9"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/22
Content-Type: application/json
Authorization: Bearer 6db1e98575901fa6ff7681a7338f9fe8c1decb3d32ae8adcdb48558991789e35
```

`GET /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 22,
    "obfuscated_id": "V2ZFfduV4jE",
    "author_id": 70,
    "chapter_id": 22,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:15:57.687Z",
    "created_at": "2016-09-08T12:15:57.687Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "<p>I'm the content</p>",
    "back_content_html": "<p>I'm the content</p>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6db1e98575901fa6ff7681a7338f9fe8c1decb3d32ae8adcdb48558991789e35"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/24/report
Content-Type: application/json
Authorization: Bearer ccf4c84682d3786a015197afdd96586cf70275d622e5abb7323b1a7f66e061c8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccf4c84682d3786a015197afdd96586cf70275d622e5abb7323b1a7f66e061c8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/16/bookmark
Content-Type: application/json
Authorization: Bearer a563ef5395052bcee913716ab9abb4d0e712206f32c7ded859ef8f5ee6362d56
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a563ef5395052bcee913716ab9abb4d0e712206f32c7ded859ef8f5ee6362d56"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/26
Content-Type: application/json
Authorization: Bearer b098ffde0b8185a5be73d41b1d79e9ceeeabdef3e6462b5a1df496f62431099e
```

`PATCH /v2/flashcards/:flashcard_id`

#### Parameters


```json
{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content]  | Front Content Markdown |
| flashcard[front_content_html]  | Front Content HTML |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[back_content_html]  | Back Content HTML |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 26,
    "obfuscated_id": "cWAsrz6MOVI",
    "author_id": 82,
    "chapter_id": 26,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:15:59.515Z",
    "created_at": "2016-09-08T12:15:59.308Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "*rise*",
    "front_content_html": "<p>I'm the content</p>",
    "back_content_html": "<strong>rise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/26" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b098ffde0b8185a5be73d41b1d79e9ceeeabdef3e6462b5a1df496f62431099e"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/25
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 3b70ba85d9c5396643fc5fd5b360367e55d0f40d71586e2111b10ca2c127094d
```

`PATCH /v2/flashcards/:flashcard_id`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

de
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content]  | Front Content Markdown |
| flashcard[front_content_html]  | Front Content HTML |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[back_content_html]  | Back Content HTML |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 25,
    "obfuscated_id": "HsmcIJXdRE4",
    "author_id": 79,
    "chapter_id": 25,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:15:59.159Z",
    "created_at": "2016-09-08T12:15:58.846Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/7d679eabdcf91345bfb62d1bc33b5d9ce650f947.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/15a055198dcce3a7fe7628bbfec0b9d1141b8251.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/7d679eabdcf91345bfb62d1bc33b5d9ce650f947.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/15a055198dcce3a7fe7628bbfec0b9d1141b8251.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/25" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

de
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 3b70ba85d9c5396643fc5fd5b360367e55d0f40d71586e2111b10ca2c127094d"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/20/upvote
Content-Type: application/json
Authorization: Bearer b174677107645c691b5a4cb819dd16fb8697052c5dca17a156a7dc9f0445fe1b
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/20/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b174677107645c691b5a4cb819dd16fb8697052c5dca17a156a7dc9f0445fe1b"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/flashcards/images/cache/presign
Content-Type: application/json
Authorization: Bearer 34e88c71fe171b8a0cc19667db503e08c3cc758e868254e93d9a04fb0f9fb0b6
```

`GET /v2/flashcards/images/cache/presign`

#### Parameters


None known.


### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/13770e2101ec90615385fa9df32876d8",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOS0wOFQxMzoxNTo1NloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8xMzc3MGUyMTAxZWM5MDYxNTM4NWZhOWRmMzI4NzZkOCJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwOTA4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDkwOFQxMjE1NTZaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160908/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160908T121556Z",
    "x-amz-signature": "87b15007c805730a81a6621031c0cb54a95f6e00a1a44d79d0f58df249a1576a"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/images/cache/presign" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34e88c71fe171b8a0cc19667db503e08c3cc758e868254e93d9a04fb0f9fb0b6"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/6/sign_ups
Content-Type: application/json
Authorization: Bearer 1c58c7e844a9c6c14ba7b6583aa64725c07cc94c35b2bb5ecd25cf7de706d705
```

`POST /v2/me/jobs/:job_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":"joe@megacorp.com"}}
```


| Name | Description |
|:-----|:------------|
| job_posting[email_address] *required* | Email to sign up with |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "sign_up": {
    "id": 2,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/6/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c58c7e844a9c6c14ba7b6583aa64725c07cc94c35b2bb5ecd25cf7de706d705"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/4/sign_ups
Content-Type: application/json
Authorization: Bearer b88a20df1117f728274399bd7bbb4f83edd31b1498d0ca9762770efe2510fba3
```

`POST /v2/me/jobs/:job_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":""}}
```


| Name | Description |
|:-----|:------------|
| job_posting[email_address] *required* | Email to sign up with |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "email_address": [
      "can't be blank"
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/4/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b88a20df1117f728274399bd7bbb4f83edd31b1498d0ca9762770efe2510fba3"
```
# Password

## Change password


### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"reset_password_token":"wWiqf4hQEcv3kTv1kfYv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "id": 594,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-09-08T12:16:38.433Z",
  "updated_at": "2016-09-08T12:16:39.276Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "downloaded_courses_count": 0,
  "university_id": null,
  "locale": "en",
  "phone_number": null,
  "phone_number_country_code": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "study_level": null,
  "audit_id": 4395
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"wWiqf4hQEcv3kTv1kfYv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
	-H "Content-Type: application/json"
```
## Change password


### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"reset_password_token":"9SCCHX3yHwLdW4BVM8B-","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "id": 1,
  "email": "jan.meier@hotmail.de",
  "created_at": "2016-09-08T12:16:40.842Z",
  "updated_at": "2016-09-08T12:16:40.998Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "downloaded_courses_count": 0,
  "university_id": null,
  "locale": "en",
  "phone_number": null,
  "phone_number_country_code": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "study_level": null,
  "audit_id": 4400
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"9SCCHX3yHwLdW4BVM8B-","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
	-H "Content-Type: application/json"
```
## Request password reset email with correct email


### Request

#### Endpoint

```
POST /v2/password
Content-Type: application/json
```

`POST /v2/password`

#### Parameters


```json
{"password":{"email":"jan.turnosky@hotmail.sk"}}
```


| Name | Description |
|:-----|:------------|
| password[email] *required* | Email address |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```




```shell
curl "api.goskive.com/v2/password" -d '{"password":{"email":"jan.turnosky@hotmail.sk"}}' -X POST \
	-H "Content-Type: application/json"
```
## Request password reset email with incorrect email


### Request

#### Endpoint

```
POST /v2/password
Content-Type: application/json
```

`POST /v2/password`

#### Parameters


```json
{"password":{"email":"jan.turnosky@hotmail.com"}}
```


| Name | Description |
|:-----|:------------|
| password[email] *required* | Email address |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```




```shell
curl "api.goskive.com/v2/password" -d '{"password":{"email":"jan.turnosky@hotmail.com"}}' -X POST \
	-H "Content-Type: application/json"
```
## Validation error on password change

An incorrect `reset_password_token` gives a validation
          error.

### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"password":"new-passw0rd","password_confirmation":"new-passw0rd","reset_password_token":"invalidt0ken"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "reset_password_token": [
      "is invalid"
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"password":"new-passw0rd","password_confirmation":"new-passw0rd","reset_password_token":"invalidt0ken"}}' -X PUT \
	-H "Content-Type: application/json"
```
# Question Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/questions/18/comments
Content-Type: application/json
Authorization: Bearer 8891980c5812335e62c32acfd2a8ba175aa00e85c530befe4480bc1ff360fb1c
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{"comment":{"message":"Not sure what this question means."}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 9,
    "author_id": 200,
    "reply_to_id": null,
    "created_at": "2016-09-08T12:16:08.929Z",
    "status": "published",
    "replies": [

    ],
    "message": "Not sure what this question means.",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/18/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8891980c5812335e62c32acfd2a8ba175aa00e85c530befe4480bc1ff360fb1c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/19/comments
Content-Type: application/json
Authorization: Bearer 2c2b14eedc301cb605bf8107d74407f041fce10465a308f7ea06057fe51a6af5
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 10,
    "author_id": 203,
    "reply_to_id": null,
    "created_at": "2016-09-08T12:16:09.287Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 10,
      "user_id": 203,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:09.285Z",
      "flags": 2,
      "message": "Really bad grammar."
    }
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/19/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c2b14eedc301cb605bf8107d74407f041fce10465a308f7ea06057fe51a6af5"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/15/comments
Content-Type: application/json
Authorization: Bearer 5f23fdd65e3beaa7e83e1858a14f3cc7c0fa186d07b43b202e691ebcde87aab4
```

`GET /v2/questions/:question_id/comments`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 8,
      "author_id": 193,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:08.329Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 192,
      "reply_to_id": null,
      "created_at": "2016-09-08T12:16:08.310Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/15/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f23fdd65e3beaa7e83e1858a14f3cc7c0fa186d07b43b202e691ebcde87aab4"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/17/comments
Content-Type: application/json
Authorization: Bearer 848919352360651e23fc5a9407aabc9a5383032236cf26bb8830a9d8846287d2
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank",
      "is too short (minimum is 2 characters)"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/17/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 848919352360651e23fc5a9407aabc9a5383032236cf26bb8830a9d8846287d2"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/7/feedbacks
Content-Type: application/json
Authorization: Bearer 739174c9bbe27f6e449e3b4762fcdb06877c0fe44cbe491a7a9dea87a576d6b6
```

`POST /v2/questions/:question_id/feedbacks`

#### Parameters


```json
{"feedback":{"message":"No comprendo","flags":0}}
```


| Name | Description |
|:-----|:------------|
| feedback[message]  | Comment message |
| feedback[flags]  | Feedback flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "feedback": {
    "id": 2,
    "user_id": 124,
    "feedbackable_id": 7,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-09-08T12:16:03.325Z",
    "flags": 0,
    "message": "No comprendo"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/7/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 739174c9bbe27f6e449e3b4762fcdb06877c0fe44cbe491a7a9dea87a576d6b6"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/12/feedbacks
Content-Type: application/json
Authorization: Bearer e9a9a958347529bb2f7420bf9633fc16da3977a1f1da95c680ab00591867a454
```

`GET /v2/questions/:question_id/feedbacks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedbacks": [
    {
      "id": 8,
      "user_id": 153,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:04.525Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 152,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-08T12:16:04.510Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/12/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9a9a958347529bb2f7420bf9633fc16da3977a1f1da95c680ab00591867a454"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/92/votes
Content-Type: application/json
Authorization: Bearer 73115cdde2cd6331f194b14a5dd0eafef775f357560b209a893da29043f89c64
```

`GET /v2/questions/:question_id/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 575
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 574
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 573
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/92/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73115cdde2cd6331f194b14a5dd0eafef775f357560b209a893da29043f89c64"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/102/republish
Content-Type: application/json
Authorization: Bearer 591bf5c03e236fd94bfa1bcd9d9773c814fe5e80201e671690145a013bc68c07
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


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
curl "api.goskive.com/v2/questions/102/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 591bf5c03e236fd94bfa1bcd9d9773c814fe5e80201e671690145a013bc68c07"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/105/bookmark
Content-Type: application/json
Authorization: Bearer 2c84bd6270e98ca58de22503a9839b7d2888259d3b8854986cec34f605fa97a7
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/105/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c84bd6270e98ca58de22503a9839b7d2888259d3b8854986cec34f605fa97a7"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/122
Content-Type: application/json
Authorization: Bearer be30e10dbfd186dbd75fb0290374bc2450f01aa8b548780f32a55043c65e11b0
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/122" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be30e10dbfd186dbd75fb0290374bc2450f01aa8b548780f32a55043c65e11b0"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/126/downvote
Content-Type: application/json
Authorization: Bearer 23c26e2ed498ac149b4c4ccac3d2c3c23bfa3cc0d9f1e825747c3faa887da470
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/126/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23c26e2ed498ac149b4c4ccac3d2c3c23bfa3cc0d9f1e825747c3faa887da470"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/125
Content-Type: application/json
Authorization: Bearer bc39f8b46c07e511e49a9b45f1559e5d39c15a212a3626f891bfec9b74a33b8e
```

`GET /v2/questions/:question_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "question": {
    "id": 125,
    "obfuscated_id": "K6zw0Yc6Me8",
    "author_id": 899,
    "chapter_id": 188,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:58.175Z",
    "created_at": "2016-09-08T12:16:58.149Z",
    "tags": [
      {
        "id": 16,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 15,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 253,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 254,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/questions/125" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc39f8b46c07e511e49a9b45f1559e5d39c15a212a3626f891bfec9b74a33b8e"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/123/report
Content-Type: application/json
Authorization: Bearer da50d729863109b7029db7d219dd635bb3b2687748eed2e00045d2530ffcbd1b
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/123/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da50d729863109b7029db7d219dd635bb3b2687748eed2e00045d2530ffcbd1b"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/124/bookmark
Content-Type: application/json
Authorization: Bearer 10c3b04be55d12b8995323cb31dade00fde340be2ed1a732c79bc7807816df9e
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/124/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10c3b04be55d12b8995323cb31dade00fde340be2ed1a732c79bc7807816df9e"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/104
Content-Type: application/json
Authorization: Bearer a0c03f750d25c5a02f7247aa9692d875b8bcdf249f9a4b7eb567527537c552f7
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":104,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-08T12:16:53.611Z","updated_at":"2016-09-08T12:16:53.639Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":167,"author_id":831,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question]  | Question Markdown |
| question[question_html]  | Question HTML |
| question[explanation]  | Explanation Markdown |
| question[explanation_html]  | Explanation HTML |
| question[answer_options]  | Answer Options |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "question": {
    "id": 104,
    "obfuscated_id": "nIg2bhYRjos",
    "author_id": 831,
    "chapter_id": 167,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-08T12:16:53.724Z",
    "created_at": "2016-09-08T12:16:53.611Z",
    "tags": [
      {
        "id": 4,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 3,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>104, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-09-08T12:16:53.611Z\", \"updated_at\"=>\"2016-09-08T12:16:53.639Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>167, \"author_id\"=>831, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 210,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 211,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 212,
        "position": 3,
        "content": "Choux needs baking powder.",
        "content_html": "<p>Choux needs baking powder.</p>",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/questions/104" -d '{"question":{"question":{"id":104,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-08T12:16:53.611Z","updated_at":"2016-09-08T12:16:53.639Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":167,"author_id":831,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0c03f750d25c5a02f7247aa9692d875b8bcdf249f9a4b7eb567527537c552f7"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/106/upvote
Content-Type: application/json
Authorization: Bearer 05becbb69de6939b3b3e4e37cc30ccb9c25c26db02a8f7cae12274b8a73da1ac
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/106/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05becbb69de6939b3b3e4e37cc30ccb9c25c26db02a8f7cae12274b8a73da1ac"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 9927b3b2591f8b268a8d00c00b389ba507083d21a096c09293f9013d7088a873
```

`GET /v2/search/courses`

#### Parameters


```json
query: Pi
```


| Name | Description |
|:-----|:------------|
| query *required* | Search query |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 303,
      "id": 87,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 94,
      "additional_university_ids": [

      ],
      "topic_id": 94,
      "discipline_id": 95,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Pizza 201",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:17.069Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9927b3b2591f8b268a8d00c00b389ba507083d21a096c09293f9013d7088a873"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 0cdadfcfec58e8bde93322092198cbe3ecddc8b052b0a9f794ff3663bc543cfc
```

`GET /v2/search/universities`

#### Parameters


```json
query: NSP
```


| Name | Description |
|:-----|:------------|
| query *required* | Search query |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "universities": [
    {
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-90",
      "html_url": "https://goskive.com/university/uni-90",
      "slug": "uni-90",
      "name": "National School of Pizza",
      "short_name": "Uni 90",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b3ea3d00a2d8319ab945fe9e5e810ffa19a4d3bd.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e1569ad6c3d0aedaf265cb53f0e148deb76c43ab.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-08T12:16:16.796Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 91,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-89",
      "html_url": "https://goskive.com/university/uni-89",
      "slug": "uni-89",
      "name": "National School of Pastry",
      "short_name": "Uni 89",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0acbb8c8fa3ee80c22c483f268ba1d99f253aa4e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b2cf275a516a5fe6923a38239128ad7a28df233b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-08T12:16:16.780Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/universities?query=NSP" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cdadfcfec58e8bde93322092198cbe3ecddc8b052b0a9f794ff3663bc543cfc"
```
# Topics

## Get a list of topics


### Request

#### Endpoint

```
GET /v2/topics
Content-Type: application/json
```

`GET /v2/topics`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "topics": [
    {
      "id": 304,
      "name": "Self-enabling value-added hub",
      "name_translations": {
        "en": "Self-enabling value-added hub"
      },
      "discipline_id": 305
    },
    {
      "id": 305,
      "name": "Synchronised user-facing concept",
      "name_translations": {
        "en": "Synchronised user-facing concept"
      },
      "discipline_id": 306
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/topics" -X GET \
	-H "Content-Type: application/json"
```
## Get a topic and translations


### Request

#### Endpoint

```
GET /v2/topics/303
Content-Type: application/json
```

`GET /v2/topics/:topic_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "topic": {
    "id": 303,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 304
  }
}
```



```shell
curl "api.goskive.com/v2/topics/303" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 7e903309272ca901fed378106ad67b4afb85bcae5178819862ae7d20cedd4b92
```

`GET /v2/universities`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "universities": [
    {
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-27",
      "html_url": "https://goskive.com/university/uni-27",
      "slug": "uni-27",
      "name": "University 27",
      "short_name": "Uni 27",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/304ae157986dd569dea48362e51bee432e419196.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cf72c04ee41f93c5e3de90878b17dec10f89dee7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-08T12:15:59.623Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-28",
      "html_url": "https://goskive.com/university/uni-28",
      "slug": "uni-28",
      "name": "University 28",
      "short_name": "Uni 28",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe4573e6024e1dcbb559e8c92df9bcbf0b713f1d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/62dc2fbffc76c59220d7254a885c01bfc78a3d58.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-08T12:15:59.639Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-29",
      "html_url": "https://goskive.com/university/uni-29",
      "slug": "uni-29",
      "name": "University 29",
      "short_name": "Uni 29",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e52f886204f3c268b5bc9c997ace9d06b6d5e0ed.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6cf2910b81a03d0b5a18d72f6ff8a336bcef109e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-08T12:15:59.655Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e903309272ca901fed378106ad67b4afb85bcae5178819862ae7d20cedd4b92"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 3b74a25239dc62b17e0a767c77b47da153fa5f2e1528103a58f125709abdb248
```

`GET /v2/universities/:university_slug`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "university": {
    "id": 31,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0b535ca5da2e9b29b5fbc2937a72466afa2de998.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f2aa41db8d47b411c27b0c58cd6fdb58f76e09ba.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-09-08T12:15:59.823Z",
    "url": "http://www.fu-berlin.de",
    "latitude": "52.496403",
    "longitude": "13.357812",
    "published": true
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b74a25239dc62b17e0a767c77b47da153fa5f2e1528103a58f125709abdb248"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0a3ef06b8bd2a5189935849b208bc932ed4c0ebcf482b96d05c4749a1a60a4dc
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":133,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
```


| Name | Description |
|:-----|:------------|
| course[title] *required* | Title |
| course[topic_id] *required* | Topic ID |
| course[chapters]  | Chapters |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |
| course[chapters][title]  | Chapter title |
| course[chapters][position]  | Chapter position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "course": {
    "creator_id": 350,
    "id": 126,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 110,
    "additional_university_ids": [

    ],
    "topic_id": 133,
    "discipline_id": 134,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 3,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-08T12:16:21.073Z",
    "updated_at": "2016-09-08T12:16:21.080Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 73,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-09-08T12:16:21.043Z",
        "course_id": 126,
        "author_id": 350,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 74,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-09-08T12:16:21.058Z",
        "course_id": 126,
        "author_id": 350,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 75,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-09-08T12:16:21.073Z",
        "course_id": 126,
        "author_id": 350,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":133,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a3ef06b8bd2a5189935849b208bc932ed4c0ebcf482b96d05c4749a1a60a4dc"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer aa1d01d5aa700f13b30e477b4561d2f060b60cbc572b57975d46b5dbf54ea20e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":134,"published":false}}
```


| Name | Description |
|:-----|:------------|
| course[title] *required* | Title |
| course[topic_id] *required* | Topic ID |
| course[chapters]  | Chapters |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |
| course[chapters][title]  | Chapter title |
| course[chapters][position]  | Chapter position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "course": {
    "creator_id": 351,
    "id": 127,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 111,
    "additional_university_ids": [

    ],
    "topic_id": 134,
    "discipline_id": 135,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-09-08T12:16:21.248Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":134,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa1d01d5aa700f13b30e477b4561d2f060b60cbc572b57975d46b5dbf54ea20e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ba22caaec63a6353b4a088a4c488fa225e374beaa8d949f19b257f1b2c509a09
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 330,
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-85",
      "html_url": "https://goskive.com/course/fu-course-85",
      "slug": "fu-course-85",
      "university_id": 102,
      "additional_university_ids": [

      ],
      "topic_id": 115,
      "discipline_id": 116,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 85",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:19.344Z",
      "shortname": "fu-course-85"
    },
    {
      "creator_id": 330,
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-86",
      "html_url": "https://goskive.com/course/fu-course-86",
      "slug": "fu-course-86",
      "university_id": 102,
      "additional_university_ids": [

      ],
      "topic_id": 116,
      "discipline_id": 117,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 86",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-09-08T12:16:19.528Z",
      "updated_at": "2016-09-08T12:16:19.531Z",
      "shortname": "fu-course-86"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba22caaec63a6353b4a088a4c488fa225e374beaa8d949f19b257f1b2c509a09"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: 
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 340,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-93",
      "html_url": "https://goskive.com/course/fu-course-93",
      "slug": "fu-course-93",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 123,
      "discipline_id": 124,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 93",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:20.113Z",
      "shortname": "fu-course-93"
    },
    {
      "creator_id": 340,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-94",
      "html_url": "https://goskive.com/course/fu-course-94",
      "slug": "fu-course-94",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "topic_id": 124,
      "discipline_id": 125,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 94",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-09-08T12:16:20.281Z",
      "updated_at": "2016-09-08T12:16:20.283Z",
      "shortname": "fu-course-94"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 285a8c0883efc2296d6f31e4390f47eb4b5fc0077aeeded6374f2722031ae720
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 336,
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-89",
      "html_url": "https://goskive.com/course/fu-course-89",
      "slug": "fu-course-89",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 119,
      "discipline_id": 120,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:19.767Z",
      "shortname": "fu-course-89"
    },
    {
      "creator_id": 336,
      "id": 113,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-90",
      "html_url": "https://goskive.com/course/fu-course-90",
      "slug": "fu-course-90",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 120,
      "discipline_id": 121,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 90",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:19.809Z",
      "shortname": "fu-course-90"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 285a8c0883efc2296d6f31e4390f47eb4b5fc0077aeeded6374f2722031ae720"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: 
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 345,
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-97",
      "html_url": "https://goskive.com/course/fu-course-97",
      "slug": "fu-course-97",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "topic_id": 127,
      "discipline_id": 128,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 97",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:20.482Z",
      "shortname": "fu-course-97"
    },
    {
      "creator_id": 345,
      "id": 121,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "topic_id": 128,
      "discipline_id": 129,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-08T12:16:20.525Z",
      "shortname": "fu-course-98"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer b20c905dd8ad9109f89fbde1a0dcd53e7b2a2ddcafe80cc6a5f15a632dc59979
```

`POST /users`

#### Parameters


```json
{"authentication_type":"password","email":"jan.turnosky@hotmail.cz","first_name":"Jan","last_name":"Turnosky","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| authentication_type *required* | Authentication Type |
| email *required* | Email address |
| first_name *required* | First name |
| last_name *required* | Last name |
| password *required* | Password |
| locale  | Locale |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "id": 405,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-09-08T12:16:24.616Z",
  "all_access_pass": false,
  "eligible_for_first_course_purchase_discount": false,
  "email": "jan.turnosky@hotmail.cz",
  "display_name": "Jan Turnosky",
  "course_ids": [

  ]
}
```



```shell
curl "api.goskive.com/users" -d '{"authentication_type":"password","email":"jan.turnosky@hotmail.cz","first_name":"Jan","last_name":"Turnosky","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b20c905dd8ad9109f89fbde1a0dcd53e7b2a2ddcafe80cc6a5f15a632dc59979"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/823
Content-Type: application/json
Authorization: Bearer 3d0b79ad52c92a08e43effea5dcc05d2dd3ed168e27ab01111cf5d7c561a0570
```

`GET /v2/users/:user_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_profile": {
    "id": 823,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 252,
    "fields_of_study": [
      275,
      276
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-09-08T12:16:52.974Z",
    "updated_at": "2016-09-08T12:16:52.974Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/823" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d0b79ad52c92a08e43effea5dcc05d2dd3ed168e27ab01111cf5d7c561a0570"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/821
Content-Type: application/json
Authorization: Bearer fda0426c39afaffe7ab41f54cc7e1468a029be0f926ec34e026a76c19472911c
```

`GET /v2/users/:user_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_profile": {
    "id": 821,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "Magnus Ahlström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-08T12:16:52.810Z",
    "updated_at": "2016-09-08T12:16:52.810Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/821" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fda0426c39afaffe7ab41f54cc7e1468a029be0f926ec34e026a76c19472911c"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/20
Content-Type: application/json
Authorization: Bearer 92ad0137aab75b29a73f9b2539a2d9b9a5effc023b13ca3d97d943f66dca597b
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92ad0137aab75b29a73f9b2539a2d9b9a5effc023b13ca3d97d943f66dca597b"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/19
Content-Type: application/json
Authorization: Bearer 45f9adb52a0d14a87beaadac7706fb237b6cf36d51d98693adf0ca487ff88633
```

`GET /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "vote": {
    "id": 19,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 95,
    "user_id": 583
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45f9adb52a0d14a87beaadac7706fb237b6cf36d51d98693adf0ca487ff88633"
```
