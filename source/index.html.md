---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# Authentication

## Authentication error on create


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7001ddd6f16569ec7ef53a1334711e77ed7697268c353bdcd217e1f43cb59366","client_secret":"b62cd6281bfbd53e576bfedb41310c7086d255382ead3bf8c7ffad28f5a5dac7"}
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
  "error": "invalid_grant",
  "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client."
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7001ddd6f16569ec7ef53a1334711e77ed7697268c353bdcd217e1f43cb59366","client_secret":"b62cd6281bfbd53e576bfedb41310c7086d255382ead3bf8c7ffad28f5a5dac7"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OGI4YTgxOGE3NjZhOTAxYmQwYTA0ZmRkZWM1MTZiYTUyZGE1MWJiYWQwMzM3
NDE2ZjMyM2I2N2UyM2QyODcwNzpkN2U4NWEwZDc3MGRhMTYzMWVlN2RhNjM3
NGM1ZmI4OWMxYWJhYTI4OWQ0ZjY3MGFjYmRiNzFmM2Q1MmVlZGUw

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
  "error": "invalid_grant",
  "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client."
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 8b8a818a766a901bd0a04fddec516ba52da51bbad0337416f323b67e23d28707:d7e85a0d770da1631ee7da6374c5fb89c1abaa289d4f670acbdb71f3d52eede0
```
## Authentication error on create


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"0ee8ea4f6e64f42d48f1a796243b51f0a5eca7865d7d5f39ab81be7049eca37d","client_secret":"493c58285cc18d2b1b30cd4ecd50d69338412efb738258c54a29dc098d137347"}
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
  "error": "invalid_grant",
  "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client."
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"0ee8ea4f6e64f42d48f1a796243b51f0a5eca7865d7d5f39ab81be7049eca37d","client_secret":"493c58285cc18d2b1b30cd4ecd50d69338412efb738258c54a29dc098d137347"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZWU3Y2M3YWU0YzQ5ZjMyMDdkODY3MTQ2Y2ZiYzY2ODFkOTlkZTJhNjQyMGM5
MjJlOGI4MzFjNjkxNTI1ZDcwNDphZmYzMWVkYWNmMzYwYTExZjU2ZjJhOTc3
YTFkM2M4ZjFkNDZjN2EyYzE2MDljNzgyZTI3MDRiYjMxZGY1NzJj

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
  "error": "invalid_grant",
  "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client."
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
	-H "Content-Type: application/json" \
	-u ee7cc7ae4c49f3207d867146cfbc6681d99de2a6420c922e8b831c691525d704:aff31edacf360a11f56f2a977a1d3c8f1d46c7a2c1609c782e2704bb31df572c
```
## Authentication error on create


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
  "error": "invalid_grant",
  "error_description": "The provided authorization grant is invalid, expired, revoked, does not match the redirection URI used in the authorization request, or was issued to another client."
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"46f76f62d55b59a6ee1cfebd3da6765a3ca08fac32f9630b7d1c1ddbe14f267e","client_secret":"db4e2683850c6724b3ba3f091e1191bb978d615ee3cb0caab8bc4749fdc3b806"}
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
  "access_token": "fa445872940b38b42662da83d9d558b75ce2d615f05d7a0780e0e9baa36a04e6",
  "token_type": "bearer",
  "created_at": 1466798596
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"46f76f62d55b59a6ee1cfebd3da6765a3ca08fac32f9630b7d1c1ddbe14f267e","client_secret":"db4e2683850c6724b3ba3f091e1191bb978d615ee3cb0caab8bc4749fdc3b806"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MjBjODQ1ZGMwM2JhMjM0MTM0YThmNDZkNjJhZTM5MmI1YTMzOGNhOTEwOTJm
MmMwMzE2MDk3MWJlN2JhNWQ3YjoyNGZkOWVhZWJhODMwM2MzODJjOGIwYjA4
NTk1MDBkOTNmYjViYjBiMTMxNTVjZDQ4ZWJjMTZkYmY0MGY4Y2Y0

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
  "access_token": "4adb60136e0b99bab46fad0f4ba3bd7fdcb9409cdce7c5826ce64fe1bd598274",
  "token_type": "bearer",
  "created_at": 1466798598
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 20c845dc03ba234134a8f46d62ae392b5a338ca91092f2c03160971be7ba5d7b:24fd9eaeba8303c382c8b0b0859500d93fb5bb0b13155cd48ebc16dbf40f8cf4
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"f27e336e306fa6cd9ed97cdd5ccc948d185e5eb5b4b76e05f729b395676147dc","client_secret":"c24b78711d49e20caa0830cb5926fb97c697265ccd43e6a4b1bda1fbc51017eb"}
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
  "access_token": "909d9ab25c2efe894a615dcaf6d62a74573d28b56491a237b1bc6488478b365b",
  "token_type": "bearer",
  "created_at": 1466798599
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"f27e336e306fa6cd9ed97cdd5ccc948d185e5eb5b4b76e05f729b395676147dc","client_secret":"c24b78711d49e20caa0830cb5926fb97c697265ccd43e6a4b1bda1fbc51017eb"}' -X POST \
	-H "Content-Type: application/json"
```
## Validation error on create


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
Authorization: Bearer a22cf3ba9f912b97f3aa1cd89fb4dbb5a40efd58672942ff59f421d764c9e514
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
    "company_id": 6,
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
	-H "Authorization: Bearer a22cf3ba9f912b97f3aa1cd89fb4dbb5a40efd58672942ff59f421d764c9e514"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/34/flashcards
Content-Type: application/json
Authorization: Bearer 588098d019a552747ac81c3794596b605a957f5f6aee8d5b7f55186b3b760343
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":34,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content] *required* | Front Content Markdown |
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content] *required* | Back Content Markdown |
| flashcard[back_content_html] *required* | Back Content HTML |
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
    "id": 19,
    "obfuscated_id": "xt199h-LGto",
    "author_id": 179,
    "chapter_id": 34,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:48.195Z",
    "created_at": "2016-06-24T20:02:48.195Z",
    "tags": [

    ],
    "reported": false,
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
curl "api.goskive.com/v2/chapters/34/flashcards" -d '{"flashcard":{"chapter_id":34,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 588098d019a552747ac81c3794596b605a957f5f6aee8d5b7f55186b3b760343"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/33/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 6f8d6a627a4784919957040304d9e4bb25ff41888679faf5afe1d1115bd0bddc
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

33
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
| flashcard[front_content] *required* | Front Content Markdown |
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content] *required* | Back Content Markdown |
| flashcard[back_content_html] *required* | Back Content HTML |
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
    "id": 18,
    "obfuscated_id": "9KZ-wsvd6MY",
    "author_id": 176,
    "chapter_id": 33,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:47.683Z",
    "created_at": "2016-06-24T20:02:47.683Z",
    "tags": [

    ],
    "reported": false,
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/fda697d64f7c42e1834c9cfc06b6f6d1aaff2646.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/50daea201097e2c6eb105cd8bac0dda4f8ce9dd1.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/fda697d64f7c42e1834c9cfc06b6f6d1aaff2646.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/50daea201097e2c6eb105cd8bac0dda4f8ce9dd1.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/33/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

33
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
	-H "Authorization: Bearer 6f8d6a627a4784919957040304d9e4bb25ff41888679faf5afe1d1115bd0bddc"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/36/flashcards
Content-Type: application/json
Authorization: Bearer 1fb9960507a717dad5b7e59db878f87268b72d87ae87ae995cc2d335985c71d2
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 183,
      "chapter_id": 36,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:48.574Z",
      "created_at": "2016-06-24T20:02:48.574Z",
      "tags": [

      ],
      "reported": false,
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    },
    {
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 183,
      "chapter_id": 36,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:48.601Z",
      "created_at": "2016-06-24T20:02:48.601Z",
      "tags": [

      ],
      "reported": false,
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    },
    {
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 183,
      "chapter_id": 36,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:48.625Z",
      "created_at": "2016-06-24T20:02:48.625Z",
      "tags": [

      ],
      "reported": false,
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/36/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fb9960507a717dad5b7e59db878f87268b72d87ae87ae995cc2d335985c71d2"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/32/questions
Content-Type: application/json
Authorization: Bearer 4b2f69111a1491f3d5f93d675b556a5840470eccedb3e8f3f44a02bb7d428b51
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":32,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 17,
    "obfuscated_id": "s3oqsdqLejU",
    "author_id": 173,
    "chapter_id": 32,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:46.286Z",
    "created_at": "2016-06-24T20:02:46.286Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 34,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 35,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 36,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 37,
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
curl "api.goskive.com/v2/chapters/32/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":32,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b2f69111a1491f3d5f93d675b556a5840470eccedb3e8f3f44a02bb7d428b51"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/30/questions
Content-Type: application/json
Authorization: Bearer 20a48284d4858edab89e3076d2af2bddd9588bfbdf3d0c6453151021bb91a82a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":30,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 15,
    "obfuscated_id": "j5PwoYQzNCc",
    "author_id": 167,
    "chapter_id": 30,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:44.900Z",
    "created_at": "2016-06-24T20:02:44.900Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 29,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 30,
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
curl "api.goskive.com/v2/chapters/30/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":30,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20a48284d4858edab89e3076d2af2bddd9588bfbdf3d0c6453151021bb91a82a"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/31/questions
Content-Type: application/json
Authorization: Bearer b5c673e25c81b7ca41c88f9f98f85e42da899a6e65ffb2596f5d6474ebfa70e6
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":31,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 16,
    "obfuscated_id": "Drq0t9y67cE",
    "author_id": 170,
    "chapter_id": 31,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:45.586Z",
    "created_at": "2016-06-24T20:02:45.586Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 31,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 32,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 33,
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
curl "api.goskive.com/v2/chapters/31/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":31,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5c673e25c81b7ca41c88f9f98f85e42da899a6e65ffb2596f5d6474ebfa70e6"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/29/questions
Content-Type: application/json
Authorization: Bearer 4ae57449dc23d74692cba3bf359d0e855b2c7983fb1fd791795309336dbf9c98
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
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 161,
      "chapter_id": 29,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:44.307Z",
      "created_at": "2016-06-24T20:02:44.272Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 23,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 24,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 162,
      "chapter_id": 29,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:44.395Z",
      "created_at": "2016-06-24T20:02:44.362Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 25,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 26,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 163,
      "chapter_id": 29,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-24T20:02:44.485Z",
      "created_at": "2016-06-24T20:02:44.451Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 27,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 28,
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
curl "api.goskive.com/v2/chapters/29/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ae57449dc23d74692cba3bf359d0e855b2c7983fb1fd791795309336dbf9c98"
```
# Chapters

## Authorisation error on delete


### Request

#### Endpoint

```
DELETE /v2/chapters/20
Content-Type: application/json
Authorization: Bearer 1ac0bbee45444619b5a9a4d06e6de70881b34a6ca0d0fce79b530f51d2ca636f
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
curl "api.goskive.com/v2/chapters/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ac0bbee45444619b5a9a4d06e6de70881b34a6ca0d0fce79b530f51d2ca636f"
```
## Authorisation error on delete


### Request

#### Endpoint

```
DELETE /v2/chapters/21
Content-Type: application/json
Authorization: Bearer 037a980561c68e501d126626a3705815b52726a0d5a424433cc46bae25959c36
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
curl "api.goskive.com/v2/chapters/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 037a980561c68e501d126626a3705815b52726a0d5a424433cc46bae25959c36"
```
## Authorisation error on update


### Request

#### Endpoint

```
PATCH /v2/chapters/26
Content-Type: application/json
Authorization: Bearer 38340f06c783e34676fec817f8f3b9a563e2eb79ec2c9ad2e66562a3bb845dca
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
curl "api.goskive.com/v2/chapters/26" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38340f06c783e34676fec817f8f3b9a563e2eb79ec2c9ad2e66562a3bb845dca"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/22
Content-Type: application/json
Authorization: Bearer 59d73ac7d0354726e45ecf904673ae782b43f9efbbded9dada8dac4fc88b4c2f
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59d73ac7d0354726e45ecf904673ae782b43f9efbbded9dada8dac4fc88b4c2f"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/24
Content-Type: application/json
Authorization: Bearer 61d77898a4fbce475776fabcc5b74bb2a534378536c2b49dc00a9926ca459f7a
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
    "id": 24,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-06-24T20:02:43.213Z",
    "course_id": 35,
    "author_id": 142,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 146,
        "chapter_id": 24,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-06-24T20:02:43.207Z",
        "tags": [

        ],
        "reported": false,
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ],
    "questions": [
      {
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 144,
        "chapter_id": 24,
        "position": 11,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-06-24T20:02:43.061Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 21,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 22,
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
curl "api.goskive.com/v2/chapters/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61d77898a4fbce475776fabcc5b74bb2a534378536c2b49dc00a9926ca459f7a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/25
Content-Type: application/json
Authorization: Bearer 27de3b84833f284d43e4fc922a693b6c042ed65081a108b50c8fb25c7b592d72
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
    "id": 25,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-06-24T20:02:43.495Z",
    "course_id": 36,
    "author_id": 149,
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
curl "api.goskive.com/v2/chapters/25" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27de3b84833f284d43e4fc922a693b6c042ed65081a108b50c8fb25c7b592d72"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/6/replies
Content-Type: application/json
Authorization: Bearer 30220aaaa8616406186dec95fa1b1ea96af3d49a2ce5909ab629cfbc0b3e31c5
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
    "id": 7,
    "author_id": 121,
    "reply_to_id": 6,
    "created_at": "2016-06-24T20:02:40.872Z",
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
curl "api.goskive.com/v2/comments/6/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30220aaaa8616406186dec95fa1b1ea96af3d49a2ce5909ab629cfbc0b3e31c5"
```
## Validation error on create


### Request

#### Endpoint

```
POST /v2/comments/5/replies
Content-Type: application/json
Authorization: Bearer a35c19f1b50f622a9cb8ef2908a55c1d20215667b6a0c51391878de3a15d5643
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
curl "api.goskive.com/v2/comments/5/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a35c19f1b50f622a9cb8ef2908a55c1d20215667b6a0c51391878de3a15d5643"
```
# Comments

## Authorisation error on delete


### Request

#### Endpoint

```
DELETE /v2/comments/19
Content-Type: application/json
Authorization: Bearer c78e3f1c47ce44da431916570c602df3e0184760bc85425d86733cd5f7144614
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
curl "api.goskive.com/v2/comments/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c78e3f1c47ce44da431916570c602df3e0184760bc85425d86733cd5f7144614"
```
## Authorisation error on republish


### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer 9312e8bec321bce05de8746d5a5a290f49e9e2acd00e257b8c63d7aa8da4147f
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
curl "api.goskive.com/v2/comments/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9312e8bec321bce05de8746d5a5a290f49e9e2acd00e257b8c63d7aa8da4147f"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/18
Content-Type: application/json
Authorization: Bearer b5108c3f910466bfa1671ded57effdbaa59b3125e2a4cdf9bfea84a10d1caab1
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5108c3f910466bfa1671ded57effdbaa59b3125e2a4cdf9bfea84a10d1caab1"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/22/report
Content-Type: application/json
Authorization: Bearer a4da41ca3b04a70bc64b405edf974772909b76e818e42aa404722a1317ea9358
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4da41ca3b04a70bc64b405edf974772909b76e818e42aa404722a1317ea9358"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/15
Content-Type: application/json
Authorization: Bearer 46360fb280404daf33f3db119baa74cdce43201c2687deb69044f6c7bc4f8f5c
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
    "id": 15,
    "name": "Pastry Corp",
    "logo_url": null,
    "brand_color": "#ffcc00",
    "updated_at": "2016-06-24T20:03:37.300Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46360fb280404daf33f3db119baa74cdce43201c2687deb69044f6c7bc4f8f5c"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer d013e51cfc8fcaff39f75c3e4f5cab9060b2bcae27f0077e4ebd4d5cbd52dd77
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
      "id": 16,
      "name": "Fake Company Name 14",
      "logo_url": null,
      "brand_color": "#000000",
      "updated_at": "2016-06-24T20:03:37.454Z"
    },
    {
      "id": 17,
      "name": "Fake Company Name 15",
      "logo_url": null,
      "brand_color": "#000000",
      "updated_at": "2016-06-24T20:03:37.459Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 16",
      "logo_url": null,
      "brand_color": "#000000",
      "updated_at": "2016-06-24T20:03:37.465Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d013e51cfc8fcaff39f75c3e4f5cab9060b2bcae27f0077e4ebd4d5cbd52dd77"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/20/company_profiles
Content-Type: application/json
Authorization: Bearer 9d1d78c52083d88ec94f1dacb237eb761db3f1328ab3d0ac613a3204ea3ef6b5
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
      "id": 7,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/9d765d9b895a77cd295c7f5e57af933f977bb87f.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/648481f5d8c76852bca2fea2b305e3b694878255.png",
      "widgets": [

      ]
    },
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 6,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/e454a32c998f7d7ac27f091147bbb511cdb6f8e8.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/0d72c01d65a8bf6733c1fdf8c672243b6d546a9e.png",
      "widgets": [

      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/20/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d1d78c52083d88ec94f1dacb237eb761db3f1328ab3d0ac613a3204ea3ef6b5"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/19/company_profiles
Content-Type: application/json
Authorization: Bearer 7e4a9cb69aae0bd4cabbf6980179e88e66573a02db49986a04cae6d270119067
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
      "id": 3,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/3e3de85f9259343d03d531c0557570e70612c274.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/9df145d07eb8d34190b3b56db5884a14a6e7644c.png",
      "widgets": [
        {
          "id": 3,
          "type": "sign_up",
          "prompt": "Sign up for the latest",
          "button_title": "Trust us",
          "confirmation_text": "Thanks for signing up"
        },
        {
          "id": 4,
          "type": "twitter",
          "prompt": "Check us out on Twitter",
          "username": "SkiveApp",
          "fallback_url": "https://goskive.com"
        },
        {
          "id": 21474836520000,
          "title": "IT Opportunity of a Lifetime",
          "description": "You cannot afford not to work for us.",
          "category": "Jobs of a Lifetime",
          "department": "BigCorp IT",
          "city_name": "München",
          "image_url": "http://company.com/image.jpg",
          "target_url": "http://company.com/",
          "pdf_url": "http://company.com/job-of-lifetime.pdf",
          "screens": [

          ],
          "company_id": 19,
          "company": {
            "id": 19,
            "name": "Pastry Corp",
            "logo_url": null,
            "brand_color": "#ffcc00",
            "updated_at": "2016-06-24T20:03:48.819Z"
          },
          "created_at": "2016-06-24T20:03:48.854Z",
          "updated_at": "2016-06-24T20:03:48.854Z",
          "type": "job_posting"
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/19/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e4a9cb69aae0bd4cabbf6980179e88e66573a02db49986a04cae6d270119067"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 833d9cb048596f8f718f6351841d191a7fd303b9672851eb6707021bc08fcf5d
```

`GET /v2/courses/:course_slug_or_id/campaigns`

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
      "id": 6,
      "title": "Campaign 5",
      "company_id": 11,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [

      ],
      "banners": [

      ]
    },
    {
      "id": 9,
      "title": "Campaign 8",
      "company_id": 14,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [

      ],
      "banners": [

      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 833d9cb048596f8f718f6351841d191a7fd303b9672851eb6707021bc08fcf5d"
```
# Course Chapters

## Authorisation error on create


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer dca9ea8413e22e5cf5ae0e8bfbfd6e6b07b0f476aa30ca02a967aa9e05737678
```

`POST /v2/courses/:course_slug_or_id/chapters`

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
	-H "Authorization: Bearer dca9ea8413e22e5cf5ae0e8bfbfd6e6b07b0f476aa30ca02a967aa9e05737678"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2ad05908dc90eb3a2f3f091cf582b92fbd344a787b66a1c084d187b31ea28412
```

`POST /v2/courses/:course_slug_or_id/chapters`

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
    "id": 38,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-06-24T20:02:49.179Z",
    "course_id": 50,
    "author_id": 191,
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
	-H "Authorization: Bearer 2ad05908dc90eb3a2f3f091cf582b92fbd344a787b66a1c084d187b31ea28412"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug_or_id/chapters`

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
      "id": 43,
      "title": "Clever Chapter Title 22",
      "position": 1,
      "updated_at": "2016-06-24T20:02:49.980Z",
      "course_id": 54,
      "author_id": 202,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 44,
      "title": "Clever Chapter Title 23",
      "position": 2,
      "updated_at": "2016-06-24T20:02:50.009Z",
      "course_id": 54,
      "author_id": 203,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 45,
      "title": "Clever Chapter Title 24",
      "position": 3,
      "updated_at": "2016-06-24T20:02:50.173Z",
      "course_id": 54,
      "author_id": 204,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-06-24T20:02:50.159Z",
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
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 687618a6a50038f21033d10df0608111ccefd165c97f63015b8fae9d3afef7b1
```

`GET /v2/courses/:course_slug_or_id/chapters`

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
      "id": 55,
      "title": "Clever Chapter Title 34",
      "position": 1,
      "updated_at": "2016-06-24T20:02:51.404Z",
      "course_id": 60,
      "author_id": 227,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 56,
      "title": "Clever Chapter Title 35",
      "position": 2,
      "updated_at": "2016-06-24T20:02:51.439Z",
      "course_id": 60,
      "author_id": 228,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 57,
      "title": "Clever Chapter Title 36",
      "position": 3,
      "updated_at": "2016-06-24T20:02:51.674Z",
      "course_id": 60,
      "author_id": 229,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-06-24T20:02:51.651Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 687618a6a50038f21033d10df0608111ccefd165c97f63015b8fae9d3afef7b1"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug_or_id/chapters`

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
      "id": 46,
      "title": "Clever Chapter Title 25",
      "position": 1,
      "updated_at": "2016-06-24T20:02:50.326Z",
      "course_id": 55,
      "author_id": 208,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 47,
      "title": "Clever Chapter Title 26",
      "position": 2,
      "updated_at": "2016-06-24T20:02:50.355Z",
      "course_id": 55,
      "author_id": 209,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 48,
      "title": "Clever Chapter Title 27",
      "position": 3,
      "updated_at": "2016-06-24T20:02:50.384Z",
      "course_id": 55,
      "author_id": 210,
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
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5ccb472e17d8876559020f607ed1edc37378f95ea9d2c7c2b1759f70e519f88f
```

`GET /v2/courses/:course_slug_or_id/chapters`

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
      "id": 58,
      "title": "Clever Chapter Title 37",
      "position": 1,
      "updated_at": "2016-06-24T20:02:52.085Z",
      "course_id": 62,
      "author_id": 236,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 59,
      "title": "Clever Chapter Title 38",
      "position": 2,
      "updated_at": "2016-06-24T20:02:52.114Z",
      "course_id": 62,
      "author_id": 237,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 60,
      "title": "Clever Chapter Title 39",
      "position": 3,
      "updated_at": "2016-06-24T20:02:52.144Z",
      "course_id": 62,
      "author_id": 238,
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
	-H "Authorization: Bearer 5ccb472e17d8876559020f607ed1edc37378f95ea9d2c7c2b1759f70e519f88f"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer a91242d2d73556b01b989c4bed00b67637fb11c18a5834e1b32150222406b5d4
```

`POST /v2/courses/:course_slug_or_id/course_requests`

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
    "course_id": 6,
    "user_id": 37,
    "updated_at": "2016-06-24T20:02:35.085Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a91242d2d73556b01b989c4bed00b67637fb11c18a5834e1b32150222406b5d4"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 677cda27ad15318c137147da94346a7c404b429d4dcd4f4fccc784007171ca7f
```

`GET /v2/courses/:course_slug_or_id/course_requests`

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
      "course_id": 9,
      "user_id": 45,
      "updated_at": "2016-06-24T20:02:35.561Z"
    },
    {
      "id": 7,
      "course_id": 9,
      "user_id": 46,
      "updated_at": "2016-06-24T20:02:35.582Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 677cda27ad15318c137147da94346a7c404b429d4dcd4f4fccc784007171ca7f"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer f2b8b802c820efaa794db286f03e01c2425a663a0b02ec8d5ba3f32e955947aa
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
	-H "Authorization: Bearer f2b8b802c820efaa794db286f03e01c2425a663a0b02ec8d5ba3f32e955947aa"
```
# Courses

## Authorisation error on delete


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 288cac97ad08dc8d07fb46ae434586dcd9459b548272efed8d37559685800fba
```

`DELETE /v2/courses/:course_slug_or_id`

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
	-H "Authorization: Bearer 288cac97ad08dc8d07fb46ae434586dcd9459b548272efed8d37559685800fba"
```
## Authorisation error on delete


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer af7535c534ea5fd05bf1ea3cd9e5f6d4f2e42a07d42ba89aaf1a59225aa698a8
```

`DELETE /v2/courses/:course_slug_or_id`

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
	-H "Authorization: Bearer af7535c534ea5fd05bf1ea3cd9e5f6d4f2e42a07d42ba89aaf1a59225aa698a8"
```
## Authorisation error on update


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cc93d2e794d6c960a26da6759b58ccb7f979afcef4a7f01d231f5129c4635420
```

`PATCH /v2/courses/:course_slug_or_id`

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
	-H "Authorization: Bearer cc93d2e794d6c960a26da6759b58ccb7f979afcef4a7f01d231f5129c4635420"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e40f8ee86f0db348472cdee8f3ca1def4eec03344da61c23a2f2fa4393a841c4
```

`DELETE /v2/courses/:course_slug_or_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e40f8ee86f0db348472cdee8f3ca1def4eec03344da61c23a2f2fa4393a841c4"
```
## Get a collection


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 3afdffc81fb47df2048f893c450f6fac7371d32d69f3ebe0486351727ba84464
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
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-25",
      "html_url": "https://goskive.com/university/uni-25",
      "slug": "uni-25",
      "name": "National School of Pizza",
      "short_name": "Uni 25",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/304ae157986dd569dea48362e51bee432e419196.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/cf72c04ee41f93c5e3de90878b17dec10f89dee7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-24T20:02:38.785Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-24",
      "html_url": "https://goskive.com/university/uni-24",
      "slug": "uni-24",
      "name": "National School of Pastry",
      "short_name": "Uni 24",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/89e9b153031acf375a336870bfce3a7d17ec2f1b.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/9eac444cb58170c4797dc004099a3c0ff73ea304.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-24T20:02:38.768Z",
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
	-H "Authorization: Bearer 3afdffc81fb47df2048f893c450f6fac7371d32d69f3ebe0486351727ba84464"
```
## Get a collection


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer f320abaaf03159325ad6d8eab96c070aeae80170cafdb745315a51934aaf8190
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
      "creator_id": 91,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 25,
      "discipline_id": 25,
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
      "updated_at": "2016-06-24T20:02:38.455Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f320abaaf03159325ad6d8eab96c070aeae80170cafdb745315a51934aaf8190"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 20156f9cf78368c3242bd7cb3eef94cb8ed651aae31f31aae2bbb0131fc13aab
```

`GET /v2/courses/:course_slug_or_id`

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
    "creator_id": 598,
    "id": 190,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "topic_id": 197,
    "discipline_id": 197,
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
    "chapters_updated_at": "2016-06-24T20:03:33.503Z",
    "updated_at": "2016-06-24T20:03:33.531Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 150,
        "title": "Clever Chapter Title 126",
        "position": 1,
        "updated_at": "2016-06-24T20:03:33.460Z",
        "course_id": 190,
        "author_id": 598,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-24T20:03:33.353Z",
        "questions_updated_at": "2016-06-24T20:03:32.928Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 151,
        "title": "Clever Chapter Title 127",
        "position": 2,
        "updated_at": "2016-06-24T20:03:33.503Z",
        "course_id": 190,
        "author_id": 598,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-24T20:03:33.411Z",
        "questions_updated_at": "2016-06-24T20:03:33.102Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 599,
        "chapter_id": 150,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.320Z",
        "created_at": "2016-06-24T20:03:33.320Z",
        "tags": [

        ],
        "reported": false,
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 599,
        "chapter_id": 151,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.380Z",
        "created_at": "2016-06-24T20:03:33.380Z",
        "tags": [

        ],
        "reported": false,
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 599,
        "chapter_id": 150,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.353Z",
        "created_at": "2016-06-24T20:03:33.353Z",
        "tags": [

        ],
        "reported": false,
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 599,
        "chapter_id": 151,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.411Z",
        "created_at": "2016-06-24T20:03:33.411Z",
        "tags": [

        ],
        "reported": false,
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ],
    "questions": [
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 599,
        "chapter_id": 150,
        "position": 66,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:32.817Z",
        "created_at": "2016-06-24T20:03:32.770Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 173,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 174,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 599,
        "chapter_id": 150,
        "position": 67,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:32.928Z",
        "created_at": "2016-06-24T20:03:32.880Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 175,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 176,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 599,
        "chapter_id": 151,
        "position": 68,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.022Z",
        "created_at": "2016-06-24T20:03:32.988Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 177,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 178,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 599,
        "chapter_id": 151,
        "position": 69,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:33.102Z",
        "created_at": "2016-06-24T20:03:33.067Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 179,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 180,
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
	-H "Authorization: Bearer 20156f9cf78368c3242bd7cb3eef94cb8ed651aae31f31aae2bbb0131fc13aab"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug_or_id`

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
    "creator_id": 593,
    "id": 189,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 174,
    "additional_university_ids": [

    ],
    "topic_id": 196,
    "discipline_id": 196,
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
    "chapters_updated_at": "2016-06-24T20:03:32.444Z",
    "updated_at": "2016-06-24T20:03:32.448Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 148,
        "title": "Clever Chapter Title 124",
        "position": 1,
        "updated_at": "2016-06-24T20:03:32.377Z",
        "course_id": 189,
        "author_id": 593,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-24T20:03:32.133Z",
        "questions_updated_at": "2016-06-24T20:03:31.216Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 149,
        "title": "Clever Chapter Title 125",
        "position": 2,
        "updated_at": "2016-06-24T20:03:32.444Z",
        "course_id": 189,
        "author_id": 593,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-24T20:03:32.236Z",
        "questions_updated_at": "2016-06-24T20:03:31.515Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 593,
        "chapter_id": 148,
        "position": 60,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:31.216Z",
        "created_at": "2016-06-24T20:03:31.159Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 161,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 162,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 593,
        "chapter_id": 149,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-24T20:03:31.515Z",
        "created_at": "2016-06-24T20:03:31.453Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 165,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 166,
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
## Get an empty list


### Request

#### Endpoint

```
GET /v2/search/universities?query=un
Content-Type: application/json
Authorization: Bearer ffd46f6c65904fd5825e5101b0bc585db5f260033b3f00e1ef16dda19004ca52
```

`GET /v2/search/universities`

#### Parameters


```json
query: un
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

  ]
}
```



```shell
curl "api.goskive.com/v2/search/universities?query=un" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffd46f6c65904fd5825e5101b0bc585db5f260033b3f00e1ef16dda19004ca52"
```
## Get an empty list


### Request

#### Endpoint

```
GET /v2/search/courses?query=un
Content-Type: application/json
Authorization: Bearer 49d43a269bb53ca7bb7e43c8e2feb22f099051eef034a320fe0072fdaec8bdff
```

`GET /v2/search/courses`

#### Parameters


```json
query: un
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

  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=un" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49d43a269bb53ca7bb7e43c8e2feb22f099051eef034a320fe0072fdaec8bdff"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/192/pin
Content-Type: application/json
Authorization: Bearer 12b1fd4d93a9f857c7b6da2ca20d815ee06a646983211b691172933e8559391e
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/192/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12b1fd4d93a9f857c7b6da2ca20d815ee06a646983211b691172933e8559391e"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/193/pin
Content-Type: application/json
Authorization: Bearer 86a321d1c9bdaf58c0da2fbe07d39adeb184cdafcfac26b8b0cf187bd472ebf3
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/193/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86a321d1c9bdaf58c0da2fbe07d39adeb184cdafcfac26b8b0cf187bd472ebf3"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3b2da4481255d2f7cc4e334d94071c87b11205c3ceaf29fca50030bd29b657ae
```

`PATCH /v2/courses/:course_slug_or_id`

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
    "creator_id": 614,
    "id": 194,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 179,
    "additional_university_ids": [

    ],
    "topic_id": 201,
    "discipline_id": 201,
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
    "updated_at": "2016-06-24T20:03:34.977Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b2da4481255d2f7cc4e334d94071c87b11205c3ceaf29fca50030bd29b657ae"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1ee630c1459e96a99a39dc25cf80638456042d089ae2af50c1c5d85d1243812f
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
    "id": 1,
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
    "created_at": "2016-06-24T20:02:19.999Z",
    "updated_at": "2016-06-24T20:02:19.999Z",
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
	-H "Authorization: Bearer 1ee630c1459e96a99a39dc25cf80638456042d089ae2af50c1c5d85d1243812f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 775888831bf1ea7a85ab31676d6d6d5c7bcb3f85650b17c23ecf162cc6fcff54
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[1]}
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
    "id": 2,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      1
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-24T20:02:20.526Z",
    "updated_at": "2016-06-24T20:02:20.609Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[1]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 775888831bf1ea7a85ab31676d6d6d5c7bcb3f85650b17c23ecf162cc6fcff54"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 84c76cf0a02e99bd2e05ec76d6923e5b77fb9ca71609ad5c222640cf1ccdd823
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
    "id": 3,
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
    "created_at": "2016-06-24T20:02:20.658Z",
    "updated_at": "2016-06-24T20:02:20.658Z",
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
	-H "Authorization: Bearer 84c76cf0a02e99bd2e05ec76d6923e5b77fb9ca71609ad5c222640cf1ccdd823"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d31cfce0e8e623ce6208b66d682cd1544bd3043cf80239d079f0f86e85ba8392
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[3]}
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
    "id": 4,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      3
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-24T20:02:20.863Z",
    "updated_at": "2016-06-24T20:02:20.863Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[3]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d31cfce0e8e623ce6208b66d682cd1544bd3043cf80239d079f0f86e85ba8392"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer da9b8051ec0eb27cc7f2f53e4c7ffd8632b9fc1206eaee2f190b91c9c7f0bc7b
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

5
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
    "id": 6,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/thumb/9bfa892827ac9e22be04a4e76f57e813fed0776c.jpg",
    "university_id": null,
    "fields_of_study": [
      5
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-24T20:02:21.105Z",
    "updated_at": "2016-06-24T20:02:21.502Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/original/7cdd7695ec242c4d7ba089f243564a8fc5406bd8.jpg",
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

5
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer da9b8051ec0eb27cc7f2f53e4c7ffd8632b9fc1206eaee2f190b91c9c7f0bc7b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 5dcb5e6d0da822617a0d9e3311dff7b5e355ebfbc94f21903fe5492d34b11a88
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
      "id": 2,
      "bookmarkable_id": 21,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 22,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 23,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5dcb5e6d0da822617a0d9e3311dff7b5e355ebfbc94f21903fe5492d34b11a88"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 77f3f7b7f33144a448fa8508bc960906e1f9c1ad24521ef199b24f84f1c62a16
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
      "creator_id": 649,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-142",
      "html_url": "https://goskive.com/course/mit-course-142",
      "slug": "mit-course-142",
      "university_id": 193,
      "additional_university_ids": [

      ],
      "topic_id": 218,
      "discipline_id": 218,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "updated_at": "2016-06-24T20:03:37.974Z",
      "shortname": "mit-course-142"
    },
    {
      "creator_id": 650,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-143",
      "html_url": "https://goskive.com/course/mit-course-143",
      "slug": "mit-course-143",
      "university_id": 194,
      "additional_university_ids": [

      ],
      "topic_id": 219,
      "discipline_id": 219,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
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
      "updated_at": "2016-06-24T20:03:38.079Z",
      "shortname": "mit-course-143"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77f3f7b7f33144a448fa8508bc960906e1f9c1ad24521ef199b24f84f1c62a16"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer ebacae1c4476d9646f1589a56574faceda4fa256cc5593b2d7122b78b51c7a03
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
      "id": 6,
      "title": "Job Posting4",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 17",
        "logo_url": null,
        "brand_color": "#000000",
        "updated_at": "2016-06-24T20:03:52.466Z"
      },
      "created_at": "2016-06-24T20:03:52.470Z",
      "updated_at": "2016-06-24T20:03:52.470Z"
    },
    {
      "id": 6,
      "title": "Job Posting4",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 17",
        "logo_url": null,
        "brand_color": "#000000",
        "updated_at": "2016-06-24T20:03:52.466Z"
      },
      "created_at": "2016-06-24T20:03:52.470Z",
      "updated_at": "2016-06-24T20:03:52.470Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebacae1c4476d9646f1589a56574faceda4fa256cc5593b2d7122b78b51c7a03"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer bfe5b95d9d3335b260966e750fdb2c8ecffa13393273316af5151ac58e4e7733
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
      "id": 14,
      "created_at": "2016-06-24T20:03:13.816Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 13,
      "updated_at": "2016-06-24T20:03:13.960Z",
      "author_id": "462",
      "thread_subject_id": "128",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 15,
      "created_at": "2016-06-24T20:03:13.943Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 14,
      "updated_at": "2016-06-24T20:03:13.965Z",
      "author_id": "465",
      "thread_subject_id": "129",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-06-24T20:03:14.272Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-06-24T20:03:14.272Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-06-24T20:03:14.727Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-06-24T20:03:14.727Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 18,
      "created_at": "2016-06-24T20:03:15.133Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-06-24T20:03:15.133Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 19,
      "created_at": "2016-06-24T20:03:15.503Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 58,
      "updated_at": "2016-06-24T20:03:15.503Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-06-24T20:03:15.790Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 59,
      "updated_at": "2016-06-24T20:03:15.790Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-06-24T20:03:16.013Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 60,
      "updated_at": "2016-06-24T20:03:16.013Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfe5b95d9d3335b260966e750fdb2c8ecffa13393273316af5151ac58e4e7733"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/13
Content-Type: application/json
Authorization: Bearer fe1c991fef37cc12e88210c129729c84f2ddb95a5c83d31eef26fa08b8d8bddd
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-06-24T19:53:13.000Z"}}
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
    "id": 13,
    "created_at": "2016-06-24T20:03:13.605Z",
    "read_at": "2016-06-24T19:53:13.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 12,
    "updated_at": "2016-06-24T20:03:13.675Z",
    "author_id": "458",
    "thread_subject_id": "127",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/13" -d '{"notification":{"read_at":"2016-06-24T19:53:13.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe1c991fef37cc12e88210c129729c84f2ddb95a5c83d31eef26fa08b8d8bddd"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 587bb52fd8d31e35b14dcb7d4e6f3d615ce0d9bec497ba1a650614708766c2d8
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
      "id": 4,
      "course_id": 262,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-06-24T20:03:49.773Z",
      "course_published": true,
      "updated_at": "2016-06-24T20:03:49.759Z"
    },
    {
      "id": 5,
      "course_id": 263,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-06-24T20:03:49.911Z",
      "course_published": true,
      "updated_at": "2016-06-24T20:03:49.897Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 587bb52fd8d31e35b14dcb7d4e6f3d615ce0d9bec497ba1a650614708766c2d8"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 03fe97c6bd799c34b04f4853403bc751ece98618e60eee0ab62a530aa199beb7
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
    "course_id": 267,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-06-24T20:03:50.926Z",
    "course_published": true,
    "updated_at": "2016-06-24T20:03:50.914Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03fe97c6bd799c34b04f4853403bc751ece98618e60eee0ab62a530aa199beb7"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 374812d4eb20ddf732281c3e55165ab0aef40f43033a6d535b14899888eaf47d
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
    "id": 6,
    "course_id": 264,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-06-24T20:03:50.363Z",
    "course_published": true,
    "updated_at": "2016-06-24T20:03:50.349Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 374812d4eb20ddf732281c3e55165ab0aef40f43033a6d535b14899888eaf47d"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 27c2de07eebfca3ca4eea0ec0fb2bfa5a5e3ae470d2ac1da2d24e711ded6ad15
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
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 809
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 104,
      "user_id": 809
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 809
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 106,
      "user_id": 809
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27c2de07eebfca3ca4eea0ec0fb2bfa5a5e3ae470d2ac1da2d24e711ded6ad15"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/272
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
    "id": 272,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 272,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 272
      },
      {
        "id": 273,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 272
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/272" -X GET \
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
      "id": 273,
      "name": "Fully-configurable human-resource emulation",
      "name_translations": {
        "en": "Fully-configurable human-resource emulation"
      }
    },
    {
      "id": 274,
      "name": "Customizable motivating archive",
      "name_translations": {
        "en": "Customizable motivating archive"
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
PATCH /v2/feedbacks/2/close
Content-Type: application/json
Authorization: Bearer 3603205558f2cee3578ac5f1eb81c9176c47bb47a9a02adf1d5d91c9ea90311c
```

`PATCH /v2/feedbacks/:feedback_id/close`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3603205558f2cee3578ac5f1eb81c9176c47bb47a9a02adf1d5d91c9ea90311c"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer f399582562ba28107ffadf5b070ef6bab144e654dc577034ca1402769b0a89e2
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f399582562ba28107ffadf5b070ef6bab144e654dc577034ca1402769b0a89e2"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/4
Content-Type: application/json
Authorization: Bearer 08fc0b18f6b269e06b40b6fbe0d17269b7901b437c4c94c6a45375e7a636d0e1
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
    "id": 4,
    "user_id": 68,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-06-24T20:02:36.965Z",
    "flags": 2
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
curl "api.goskive.com/v2/feedbacks/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08fc0b18f6b269e06b40b6fbe0d17269b7901b437c4c94c6a45375e7a636d0e1"
```
## Validation error on feedback state change


### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer fcdc6b61a7cc9b47d662c8d035f3868cf192e4aa4132a41106eb7daeb4204c2a
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
curl "api.goskive.com/v2/feedbacks/1/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcdc6b61a7cc9b47d662c8d035f3868cf192e4aa4132a41106eb7daeb4204c2a"
```
## Validation error on feedback state change


### Request

#### Endpoint

```
PATCH /v2/feedbacks/7/fix
Content-Type: application/json
Authorization: Bearer ce4dc6b012306ccae8041d8510dd7dbe2a02db28d2bd6d845f76b3993a9b4b47
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
curl "api.goskive.com/v2/feedbacks/7/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce4dc6b012306ccae8041d8510dd7dbe2a02db28d2bd6d845f76b3993a9b4b47"
```
## Validation error on feedback state change


### Request

#### Endpoint

```
PATCH /v2/feedbacks/8/fix
Content-Type: application/json
Authorization: Bearer bca3dd5012c3dd3e92ff9fca221933bd7046db7dcc2d4e7726220ad5eefecb66
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
curl "api.goskive.com/v2/feedbacks/8/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bca3dd5012c3dd3e92ff9fca221933bd7046db7dcc2d4e7726220ad5eefecb66"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer e75edfe891cbd39c6515d7fc921efa5ece2372fe02daffa0943de71f0a2409f0
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
    "author_id": 106,
    "reply_to_id": null,
    "created_at": "2016-06-24T20:02:39.960Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e75edfe891cbd39c6515d7fc921efa5ece2372fe02daffa0943de71f0a2409f0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer 16ec763b06ec23b8514726cc8cbce9606ffb3dd8f34e3e2e225538c0c8199652
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
    "author_id": 103,
    "reply_to_id": null,
    "created_at": "2016-06-24T20:02:39.598Z",
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 103,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:02:39.594Z",
      "flags": 3
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
curl "api.goskive.com/v2/flashcards/11/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16ec763b06ec23b8514726cc8cbce9606ffb3dd8f34e3e2e225538c0c8199652"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer 90a0f039314d0dd3a8d3241660ae38ada6ef64c9274d870fa6dc5dce50c897fb
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
      "id": 1,
      "author_id": 101,
      "reply_to_id": null,
      "created_at": "2016-06-24T20:02:39.268Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 102,
      "reply_to_id": null,
      "created_at": "2016-06-24T20:02:39.315Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/10/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90a0f039314d0dd3a8d3241660ae38ada6ef64c9274d870fa6dc5dce50c897fb"
```
## Validation error on create


### Request

#### Endpoint

```
POST /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer 36a12a3e6ac4a7ac68d95933cd0a958ff0184b23ec899eca19d064367ceb3e59
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
curl "api.goskive.com/v2/flashcards/13/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36a12a3e6ac4a7ac68d95933cd0a958ff0184b23ec899eca19d064367ceb3e59"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/92/feedbacks
Content-Type: application/json
Authorization: Bearer 7a5a066fa2d00c28866501294a5f0515c6748963376af88919c2bd545824cde8
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
    "id": 25,
    "user_id": 787,
    "feedbackable_id": 92,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-06-24T20:03:48.064Z",
    "flags": 0
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
curl "api.goskive.com/v2/flashcards/92/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a5a066fa2d00c28866501294a5f0515c6748963376af88919c2bd545824cde8"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/90/feedbacks
Content-Type: application/json
Authorization: Bearer f478cce28a57f61c8e9d84e3e1aee399972402bce18f31ebb217400e6cb1dd56
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
      "id": 24,
      "user_id": 783,
      "feedbackable_id": 90,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:03:47.640Z",
      "flags": 1
    },
    {
      "id": 23,
      "user_id": 782,
      "feedbackable_id": 90,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:03:47.624Z",
      "flags": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/90/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f478cce28a57f61c8e9d84e3e1aee399972402bce18f31ebb217400e6cb1dd56"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/53/votes
Content-Type: application/json
Authorization: Bearer 2ef5a2f1372f4f68e8cc210f9018a5326b6cc8ead8531354d91aaf0d354811bd
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
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 53,
      "user_id": 352
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 53,
      "user_id": 351
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 53,
      "user_id": 350
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ef5a2f1372f4f68e8cc210f9018a5326b6cc8ead8531354d91aaf0d354811bd"
```
# Flashcards

## Authorisation error on republish


### Request

#### Endpoint

```
PUT /v2/flashcards/49/republish
Content-Type: application/json
Authorization: Bearer 8b08577af398e84891d912832127b4f6d06398ab71f80a8e4791cdac6893b172
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
curl "api.goskive.com/v2/flashcards/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b08577af398e84891d912832127b4f6d06398ab71f80a8e4791cdac6893b172"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/29/bookmark
Content-Type: application/json
Authorization: Bearer 7dd67de8a7798ad647ad5a7c19b83f8fde3ecabcefb7a586a05fdafc042aca3c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/29/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dd67de8a7798ad647ad5a7c19b83f8fde3ecabcefb7a586a05fdafc042aca3c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50
Content-Type: application/json
Authorization: Bearer 5fd3c4dd5956a8188193099a603a990e7f09359e30800994dd99e7328856c6af
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fd3c4dd5956a8188193099a603a990e7f09359e30800994dd99e7328856c6af"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/28/downvote
Content-Type: application/json
Authorization: Bearer 42bf9329ff8d4a9744cf0f1bdae64310d7a5eb820ae34c3c6500e7c943fbb383
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42bf9329ff8d4a9744cf0f1bdae64310d7a5eb820ae34c3c6500e7c943fbb383"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/47
Content-Type: application/json
Authorization: Bearer cc0783a3e95d0e7f3bb92c5d146528b62da225aedc24ccb47e7d963284997607
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
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 312,
    "chapter_id": 82,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:57.488Z",
    "created_at": "2016-06-24T20:02:57.488Z",
    "tags": [

    ],
    "reported": false,
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
    "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc0783a3e95d0e7f3bb92c5d146528b62da225aedc24ccb47e7d963284997607"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/27/report
Content-Type: application/json
Authorization: Bearer 5e4d1f2182dbd4d24d579d79cc8469536f932cebddd98c480fc9ba0c0db35cf8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/27/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e4d1f2182dbd4d24d579d79cc8469536f932cebddd98c480fc9ba0c0db35cf8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/51/bookmark
Content-Type: application/json
Authorization: Bearer 25ed49b00d399b11b71351b1acfeed5ed7ae3ca8b99dfed7bc30c1e33cfe5d98
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/51/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25ed49b00d399b11b71351b1acfeed5ed7ae3ca8b99dfed7bc30c1e33cfe5d98"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/45
Content-Type: application/json
Authorization: Bearer e9d9f8f164731e33cf23a4cbf15c9a45809be53da2270aa14f5a3a4bb26a71e6
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
    "id": 45,
    "obfuscated_id": "IVleRnyZemc",
    "author_id": 306,
    "chapter_id": 80,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:56.541Z",
    "created_at": "2016-06-24T20:02:56.214Z",
    "tags": [

    ],
    "reported": false,
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "*rise*",
    "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
    "back_content_html": "<strong>rise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/45" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9d9f8f164731e33cf23a4cbf15c9a45809be53da2270aa14f5a3a4bb26a71e6"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/46
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer e1a0443dda4bfb6f53820c915768fbf823b3e0e8c6b9544c295ac22dded82d51
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
    "id": 46,
    "obfuscated_id": "urkHiAaH08E",
    "author_id": 309,
    "chapter_id": 81,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:02:57.275Z",
    "created_at": "2016-06-24T20:02:56.706Z",
    "tags": [

    ],
    "reported": false,
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/68557aaaf683e4c07960dc6a400c470099708864.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/1931a7f58193fcc6733648b443f6d03b5ec53b63.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/68557aaaf683e4c07960dc6a400c470099708864.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/1931a7f58193fcc6733648b443f6d03b5ec53b63.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/46" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
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
	-H "Authorization: Bearer e1a0443dda4bfb6f53820c915768fbf823b3e0e8c6b9544c295ac22dded82d51"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/upvote
Content-Type: application/json
Authorization: Bearer beceab351fefba0fd2c0b9ab42b705361e9eb6058059313b98cba7c00cabe566
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/26/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer beceab351fefba0fd2c0b9ab42b705361e9eb6058059313b98cba7c00cabe566"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer f63b5a0eb8fbbc085791a0f25a876f756360bfb59d3271660281cccc5c990584
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
    "id": 3,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/3/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f63b5a0eb8fbbc085791a0f25a876f756360bfb59d3271660281cccc5c990584"
```
## Validation error on sign up


### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 89b984d0a6a2b0ccb84f9b46d894a4d863c7b10f3b1a4219adb3a66c727ddc8b
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
curl "api.goskive.com/v2/me/jobs/1/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89b984d0a6a2b0ccb84f9b46d894a4d863c7b10f3b1a4219adb3a66c727ddc8b"
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
{"password":{"reset_password_token":"SJpNjd7JHsenz3TgoquM","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 33,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-06-24T20:02:33.218Z",
  "updated_at": "2016-06-24T20:02:34.674Z",
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
  "audit_id": 72155
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"SJpNjd7JHsenz3TgoquM","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
{"password":{"reset_password_token":"GeqWKjt38o1sHqwXCQiQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "created_at": "2016-06-24T20:02:32.971Z",
  "updated_at": "2016-06-24T20:02:33.164Z",
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
  "audit_id": 72154
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"GeqWKjt38o1sHqwXCQiQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/25/comments
Content-Type: application/json
Authorization: Bearer 38d9988faf80d49a02b8145047396dd0aa0097c8ffd45ebfdbee2f383758fff0
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
    "id": 8,
    "author_id": 356,
    "reply_to_id": null,
    "created_at": "2016-06-24T20:03:03.040Z",
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
curl "api.goskive.com/v2/questions/25/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38d9988faf80d49a02b8145047396dd0aa0097c8ffd45ebfdbee2f383758fff0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer 4a5987685fda27105bb858bfaf6ee26fc1c134ca84357f29b46fd683bc1f6e9c
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
    "id": 9,
    "author_id": 362,
    "reply_to_id": null,
    "created_at": "2016-06-24T20:03:04.315Z",
    "message": "Really bad grammar.",
    "feedback": {
      "id": 10,
      "user_id": 362,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:03:04.309Z",
      "flags": 2
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
curl "api.goskive.com/v2/questions/27/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a5987685fda27105bb858bfaf6ee26fc1c134ca84357f29b46fd683bc1f6e9c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/29/comments
Content-Type: application/json
Authorization: Bearer 1d18cf50e4bf2690e5e803af6043f9babf985bb5dfa9bef52de32cd80706ec10
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
      "id": 11,
      "author_id": 372,
      "reply_to_id": null,
      "created_at": "2016-06-24T20:03:05.315Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 371,
      "reply_to_id": null,
      "created_at": "2016-06-24T20:03:05.282Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/29/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d18cf50e4bf2690e5e803af6043f9babf985bb5dfa9bef52de32cd80706ec10"
```
## Validation error on create


### Request

#### Endpoint

```
POST /v2/questions/26/comments
Content-Type: application/json
Authorization: Bearer 01e6f7b2c1634270074e0b8bfe8b52e3d1209abf4811907dac743cd822d81944
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
curl "api.goskive.com/v2/questions/26/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01e6f7b2c1634270074e0b8bfe8b52e3d1209abf4811907dac743cd822d81944"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/68/feedbacks
Content-Type: application/json
Authorization: Bearer 9f3a0ae90e5f1dc5b9ff608c8d69a232b4829bea77245fedba8b820f9e2c6840
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
    "id": 18,
    "user_id": 531,
    "feedbackable_id": 68,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-06-24T20:03:22.560Z",
    "flags": 0
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
curl "api.goskive.com/v2/questions/68/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f3a0ae90e5f1dc5b9ff608c8d69a232b4829bea77245fedba8b820f9e2c6840"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/64/feedbacks
Content-Type: application/json
Authorization: Bearer 9f14586274bba8655baea18f689b31bee6436fc50c49a47118154d9e3e36d744
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
      "id": 14,
      "user_id": 519,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:03:21.257Z",
      "flags": 1
    },
    {
      "id": 13,
      "user_id": 518,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-24T20:03:21.241Z",
      "flags": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/64/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f14586274bba8655baea18f689b31bee6436fc50c49a47118154d9e3e36d744"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/100/votes
Content-Type: application/json
Authorization: Bearer 0403610b8b5bd1a2f12fb160ec5bb8afcee99da49c036070643d854cd6705d9e
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
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 657
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 656
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 655
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/100/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0403610b8b5bd1a2f12fb160ec5bb8afcee99da49c036070643d854cd6705d9e"
```
# Questions

## Authorisation error on republish


### Request

#### Endpoint

```
PUT /v2/questions/52/republish
Content-Type: application/json
Authorization: Bearer 13cfa24304f7e5b9150ffcbabc774de91b16bb65e64a5a7ae0b60231816771d2
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
curl "api.goskive.com/v2/questions/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13cfa24304f7e5b9150ffcbabc774de91b16bb65e64a5a7ae0b60231816771d2"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/50/bookmark
Content-Type: application/json
Authorization: Bearer bd4c9ca88f96bf64a2533bcdad192769f0b37a4405d925e172ceaae1241c9b59
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd4c9ca88f96bf64a2533bcdad192769f0b37a4405d925e172ceaae1241c9b59"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/46
Content-Type: application/json
Authorization: Bearer f3a47b28e621b7cd940c605aac99cd06474f813f7ca9437c0f96e7d59c347674
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3a47b28e621b7cd940c605aac99cd06474f813f7ca9437c0f96e7d59c347674"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/47/downvote
Content-Type: application/json
Authorization: Bearer 408cb026e67be45a3922e5576ee2783558b8e959c61238f88e76b1acce5a8976
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/47/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 408cb026e67be45a3922e5576ee2783558b8e959c61238f88e76b1acce5a8976"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/53
Content-Type: application/json
Authorization: Bearer ca481bf5b74337b3cf62956a31b383a84228ffeca485069257ca3c2794d27e77
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
    "id": 53,
    "obfuscated_id": "XffxqHkTsbc",
    "author_id": 447,
    "chapter_id": 122,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:03:12.151Z",
    "created_at": "2016-06-24T20:03:12.114Z",
    "tags": [
      {
        "id": 18,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 17,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "reported": false,
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
        "id": 109,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 110,
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
curl "api.goskive.com/v2/questions/53" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca481bf5b74337b3cf62956a31b383a84228ffeca485069257ca3c2794d27e77"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/54/report
Content-Type: application/json
Authorization: Bearer 985c4a3331dd395b8be59258169bd436deae7b0e6fc0615382e885db1f9e3958
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/54/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 985c4a3331dd395b8be59258169bd436deae7b0e6fc0615382e885db1f9e3958"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/48/bookmark
Content-Type: application/json
Authorization: Bearer 9814ad7353766fbe405ca16f8739a643acba318c201a8501857f176dc5a47c5e
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9814ad7353766fbe405ca16f8739a643acba318c201a8501857f176dc5a47c5e"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/30
Content-Type: application/json
Authorization: Bearer abea3193c981992f184a312aa4a2d219675a2593c92d50dd74ec918a84391b67
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":30,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-06-24T20:03:05.600Z","updated_at":"2016-06-24T20:03:05.640Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":99,"author_id":373,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 373,
    "chapter_id": 99,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-24T20:03:05.735Z",
    "created_at": "2016-06-24T20:03:05.600Z",
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
    "reported": false,
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>30, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-06-24T20:03:05.600Z\", \"updated_at\"=>\"2016-06-24T20:03:05.640Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>99, \"author_id\"=>373, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 62,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 63,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 64,
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
curl "api.goskive.com/v2/questions/30" -d '{"question":{"question":{"id":30,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-06-24T20:03:05.600Z","updated_at":"2016-06-24T20:03:05.640Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":99,"author_id":373,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abea3193c981992f184a312aa4a2d219675a2593c92d50dd74ec918a84391b67"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/49/upvote
Content-Type: application/json
Authorization: Bearer bf76db51d0b37488a366548c2114c1a378baba85d2ac6c6620dfe43b79405748
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf76db51d0b37488a366548c2114c1a378baba85d2ac6c6620dfe43b79405748"
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
      "id": 214,
      "name": "Seamless actuating circuit",
      "name_translations": {
        "en": "Seamless actuating circuit"
      },
      "discipline_id": 214
    },
    {
      "id": 215,
      "name": "Assimilated executive database",
      "name_translations": {
        "en": "Assimilated executive database"
      },
      "discipline_id": 215
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
GET /v2/topics/216
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
    "id": 216,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 216
  }
}
```



```shell
curl "api.goskive.com/v2/topics/216" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 9c01f661b89d75799b79bf45b006a205c77eb1b30390d3060aa1f7070c01c699
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
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-1",
      "html_url": "https://goskive.com/university/uni-1",
      "slug": "uni-1",
      "name": "University 1",
      "short_name": "Uni 1",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/0178e4c1b8a1e0379f3158851027049f94ddc463.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/51e7a1f572cf9347372a35d5e9ae2cc89f48eb30.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-24T20:02:22.144Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "University 2",
      "short_name": "Uni 2",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-24T20:02:22.161Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 5,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-3",
      "html_url": "https://goskive.com/university/uni-3",
      "slug": "uni-3",
      "name": "University 3",
      "short_name": "Uni 3",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/b0565dc08fa00cadf540ab3ebebe19c2c1549d4c.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/6d81c502295167ffd30dd07df6bdf0416bf4938f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-24T20:02:22.182Z",
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
	-H "Authorization: Bearer 9c01f661b89d75799b79bf45b006a205c77eb1b30390d3060aa1f7070c01c699"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 3f5f84d8d5407299a410eda783e784a32aaafb44eefd5390297f2bb08ba90928
```

`GET /v2/universities/:university_slug_or_id`

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
    "id": 1,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/38802f33528ba3ba141b3ec7e7bce0a2b851ee78.png",
    "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/51291693f690a69f7677e03637596dc7709b266f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-06-24T20:02:21.937Z",
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
	-H "Authorization: Bearer 3f5f84d8d5407299a410eda783e784a32aaafb44eefd5390297f2bb08ba90928"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 90890e82c58dfec5f674a5239545cef4cdc212b1b88f9c234768062e54eab701
```

`POST /v2/universities/:university_slug_or_id/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":191,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 583,
    "id": 184,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 169,
    "additional_university_ids": [

    ],
    "topic_id": 191,
    "discipline_id": 191,
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
    "chapters_updated_at": "2016-06-24T20:03:28.139Z",
    "updated_at": "2016-06-24T20:03:28.157Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 143,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-06-24T20:03:28.036Z",
        "course_id": 184,
        "author_id": 583,
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
        "id": 144,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-06-24T20:03:28.067Z",
        "course_id": 184,
        "author_id": 583,
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
        "id": 145,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-06-24T20:03:28.139Z",
        "course_id": 184,
        "author_id": 583,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":191,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90890e82c58dfec5f674a5239545cef4cdc212b1b88f9c234768062e54eab701"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 41787d00d9df8406eb86f87a42bc9148abd103c8a884c121431b1fdb20a051e5
```

`POST /v2/universities/:university_slug_or_id/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":192,"published":false}}
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
    "creator_id": 584,
    "id": 185,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 170,
    "additional_university_ids": [

    ],
    "topic_id": 192,
    "discipline_id": 192,
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
    "updated_at": "2016-06-24T20:03:28.517Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":192,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41787d00d9df8406eb86f87a42bc9148abd103c8a884c121431b1fdb20a051e5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2cd2233e784cb62883260622625174123cb23c43b555e14a1937b628005519db
```

`GET /v2/universities/:university_slug_or_id/courses`

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
      "creator_id": 570,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-06-24T20:03:26.684Z",
      "shortname": "fu-course-127"
    },
    {
      "creator_id": 570,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
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
      "chapters_updated_at": "2016-06-24T20:03:26.907Z",
      "updated_at": "2016-06-24T20:03:26.912Z",
      "shortname": "fu-course-128"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cd2233e784cb62883260622625174123cb23c43b555e14a1937b628005519db"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: 
```

`GET /v2/universities/:university_slug_or_id/courses`

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
      "creator_id": 543,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 157,
      "discipline_id": 157,
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
      "updated_at": "2016-06-24T20:03:23.807Z",
      "shortname": "fu-course-103"
    },
    {
      "creator_id": 543,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-104",
      "html_url": "https://goskive.com/course/fu-course-104",
      "slug": "fu-course-104",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 158,
      "discipline_id": 158,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
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
      "chapters_updated_at": "2016-06-24T20:03:24.073Z",
      "updated_at": "2016-06-24T20:03:24.076Z",
      "shortname": "fu-course-104"
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
Authorization: 
```

`GET /v2/universities/:university_slug_or_id/courses`

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
      "creator_id": 548,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 161,
      "discipline_id": 161,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
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
      "updated_at": "2016-06-24T20:03:24.381Z",
      "shortname": "fu-course-107"
    },
    {
      "creator_id": 548,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 162,
      "discipline_id": 162,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
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
      "updated_at": "2016-06-24T20:03:24.434Z",
      "shortname": "fu-course-108"
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
Authorization: Bearer a5f286f7101177ee2644d7c667d528fe4eb3dd6efd88b289f30423fa99c5d89f
```

`GET /v2/universities/:university_slug_or_id/courses`

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
      "creator_id": 577,
      "id": 178,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
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
      "updated_at": "2016-06-24T20:03:27.335Z",
      "shortname": "fu-course-131"
    },
    {
      "creator_id": 577,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "topic_id": 186,
      "discipline_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "updated_at": "2016-06-24T20:03:27.388Z",
      "shortname": "fu-course-132"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5f286f7101177ee2644d7c667d528fe4eb3dd6efd88b289f30423fa99c5d89f"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer abfe87e0af4f0928001e1fa54b338aaf63e1b1e8c99728f80c6b7dff5c964980
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
  "id": 27,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-06-24T20:02:23.652Z",
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
	-H "Authorization: Bearer abfe87e0af4f0928001e1fa54b338aaf63e1b1e8c99728f80c6b7dff5c964980"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/240
Content-Type: application/json
Authorization: Bearer 92624da2a6e84cb171ac2014bf2a735b1b508f009a2f7a2e9bf55f0e0ae85baa
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
    "id": 240,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 69,
    "fields_of_study": [
      68,
      69
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-06-24T20:02:52.344Z",
    "updated_at": "2016-06-24T20:02:52.344Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/240" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92624da2a6e84cb171ac2014bf2a735b1b508f009a2f7a2e9bf55f0e0ae85baa"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/242
Content-Type: application/json
Authorization: Bearer b1d1b7398576f75419144d654515124b8ce0771f56fe7ffcc8c347d936af2d7e
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
    "id": 242,
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
    "created_at": "2016-06-24T20:02:52.464Z",
    "updated_at": "2016-06-24T20:02:52.464Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/242" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1d1b7398576f75419144d654515124b8ce0771f56fe7ffcc8c347d936af2d7e"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/2
Content-Type: application/json
Authorization: Bearer 7cd176af3eb69dded3cd21e0389bcf2a129986a4a4f93981c616d293c91bdf74
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cd176af3eb69dded3cd21e0389bcf2a129986a4a4f93981c616d293c91bdf74"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/3
Content-Type: application/json
Authorization: Bearer 7299c93fa6dab41a18e4ed4968ccaa3c248306c5d6899f4eadbf0cc42c1f7a3f
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
    "id": 3,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 23
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7299c93fa6dab41a18e4ed4968ccaa3c248306c5d6899f4eadbf0cc42c1f7a3f"
```
# Widget Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/widgets/1/sign_ups
Content-Type: application/json
Authorization: Bearer 7771644f951bdd800305cfe2c1b8cf2c6ad7eafe12f46f5dd62f027567d09803
```

`POST /v2/me/widgets/:widget_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":"joe@megacorp.com"}}
```


| Name | Description |
|:-----|:------------|
| sign_up[email_address] *required* | Email address to sign up with |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "sign_up": {
    "id": 1,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/widgets/1/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7771644f951bdd800305cfe2c1b8cf2c6ad7eafe12f46f5dd62f027567d09803"
```
## Validation error on sign up


### Request

#### Endpoint

```
POST /v2/me/widgets/2/sign_ups
Content-Type: application/json
Authorization: Bearer 70d74002c1c101c15a1ced6cd2bd915751df534b84516d63012d2492e6db0254
```

`POST /v2/me/widgets/:widget_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":""}}
```


| Name | Description |
|:-----|:------------|
| sign_up[email_address] *required* | Email address to sign up with |



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
curl "api.goskive.com/v2/me/widgets/2/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70d74002c1c101c15a1ced6cd2bd915751df534b84516d63012d2492e6db0254"
```
