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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2168fa2d94a30d77e4a6977ab345edf7833bc59cd7b7f865b5671c63c32b29a8","client_secret":"f2593b3b9460f3ae0d435a39f02f3fb01a086a59f64debc6146ea3156263bfb6"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2168fa2d94a30d77e4a6977ab345edf7833bc59cd7b7f865b5671c63c32b29a8","client_secret":"f2593b3b9460f3ae0d435a39f02f3fb01a086a59f64debc6146ea3156263bfb6"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a0c8ce2301cbbfbef526e032a0b484d993dd765eafdab65571155a8ee3724ec7","client_secret":"a9669c8b9d0f6e4447c82d6ed75aa1df1ab6c6efe16ee6a50a1ae42db76ee887"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a0c8ce2301cbbfbef526e032a0b484d993dd765eafdab65571155a8ee3724ec7","client_secret":"a9669c8b9d0f6e4447c82d6ed75aa1df1ab6c6efe16ee6a50a1ae42db76ee887"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDlhNjc5M2RhZTM0NWQwZjU4ZDE0OWU3OGE1MzVmMjUwNDdlODRmZWM4MzJj
ZjYzZjIyMzkzNTIzNDI3YWEyOTpjNGZhYzlhMjJjOGI4OTlkNTA1OWNiZTI2
OTliNzU2ZTcwNTAwMjA4NzY1MWEzZWU0OWYxZDdhYzVlNTRkMzA3

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
	-u d9a6793dae345d0f58d149e78a535f25047e84fec832cf63f22393523427aa29:c4fac9a22c8b899d5059cbe2699b756e705002087651a3ee49f1d7ac5e54d307
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic M2Q5YzZkMjI4ODNmODM1MDk1NTMxZDk1NjAxMDRhODIwMWNjMDkxMTVlNDBh
ODMwM2ZmM2Q5NmQwYTFkNTg0ODo0MTc0NTVmYTgwNjYyYTFmNzgwMzY4MzA1
MDFjZGEwNTc5MGE4MTM2MDJiZWU2YTUwNjM3N2JkMTcxNmYyOWJj

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
	-u 3d9c6d22883f835095531d9560104a8201cc09115e40a8303ff3d96d0a1d5848:417455fa80662a1f78036830501cda05790a813602bee6a506377bd1716f29bc
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
{"grant_type":"client_credentials","client_id":"9cb492fc536252b3295aa4994a12d97d6728a7aa3913f8aee6f76e49ca46b5bd","client_secret":"977cad5b74c538a79fd52fe941361769d8eb5140f7ea0fe3308ef2e52f7c2f57"}
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
  "access_token": "ddc3ff98adc6d18e2b56e8cfca97709adf536dfd6c0c03c718e3007e5e54039d",
  "token_type": "bearer",
  "created_at": 1472737124
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"9cb492fc536252b3295aa4994a12d97d6728a7aa3913f8aee6f76e49ca46b5bd","client_secret":"977cad5b74c538a79fd52fe941361769d8eb5140f7ea0fe3308ef2e52f7c2f57"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cabbd8e4819c2c0b6354b705a805345ff18a32dedc0602a192ca24c2897e34e5","client_secret":"ea126506c83f61c5f2cac0d2aa7c2613c9ec75c159fce1a02f8d18f8b5726ab2"}
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
  "access_token": "17b1031a99baaf7ef5f7901c1b97b4b24f36a1f859c0b89bd9663e29c59a48c7",
  "token_type": "bearer",
  "created_at": 1472737125
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cabbd8e4819c2c0b6354b705a805345ff18a32dedc0602a192ca24c2897e34e5","client_secret":"ea126506c83f61c5f2cac0d2aa7c2613c9ec75c159fce1a02f8d18f8b5726ab2"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic N2E2ODFlMmY2NDBkZTliM2Q5M2M3ZWQ1NjM5Njg3Mjc0MTcwYzRlYjRiZmZm
OGM0ZWYxMTNhNmIzNmYyODI0MDpkNjk5MTA5Y2NhZDUwZTdlNDZkZTY5NjY3
ZTQwOTY5YmVhZTFmZTFkYWQ1ZTRiY2YxMzYzMWQzMTE0M2EyMmQy

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
  "access_token": "217a0b1ea6bc86478240a91fa4ea2eef305c22dd9b9fc7acb4f4379e90f8b31a",
  "token_type": "bearer",
  "created_at": 1472737125
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 7a681e2f640de9b3d93c7ed5639687274170c4eb4bfff8c4ef113a6b36f28240:d699109ccad50e7e46de69667e40969beae1fe1dad5e4bcf13631d31143a22d2
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
GET /v2/campaigns/11
Content-Type: application/json
Authorization: Bearer 6e38e4fcc19e572adcf37bb98d1881984d54e9a223b4f99fd36423885359e55c
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
    "id": 11,
    "title": "Recruiting pastry chefs",
    "company_id": 21,
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
curl "api.goskive.com/v2/campaigns/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e38e4fcc19e572adcf37bb98d1881984d54e9a223b4f99fd36423885359e55c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/55/flashcards
Content-Type: application/json
Authorization: Bearer 15209695ebda0ca0184e18c879217499f0b93b8e7d37a59797514ef25a1e1b00
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":55,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 333,
    "chapter_id": 55,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:37.164Z",
    "created_at": "2016-09-01T13:38:37.164Z",
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
curl "api.goskive.com/v2/chapters/55/flashcards" -d '{"flashcard":{"chapter_id":55,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15209695ebda0ca0184e18c879217499f0b93b8e7d37a59797514ef25a1e1b00"
```
## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/56/flashcards
Content-Type: application/json
Authorization: Bearer b303a234a8bb452a1bef5ee6aff280c6c1172d745af66c2f13031b10e5625eb4
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":56,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 336,
    "chapter_id": 56,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:37.606Z",
    "created_at": "2016-09-01T13:38:37.606Z",
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
curl "api.goskive.com/v2/chapters/56/flashcards" -d '{"flashcard":{"chapter_id":56,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b303a234a8bb452a1bef5ee6aff280c6c1172d745af66c2f13031b10e5625eb4"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/54/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 7bfa4e744dfa3c2d8c017a957bab99f30218132445a0ed9c2797292c12923b38
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

54
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 330,
    "chapter_id": 54,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:36.719Z",
    "created_at": "2016-09-01T13:38:36.719Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/33b021317aa9a09b0d19eb5a6d20d51f2df0a456.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/46c8d5b360186db757cef4dc7638e92cc746a8d8.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/33b021317aa9a09b0d19eb5a6d20d51f2df0a456.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/46c8d5b360186db757cef4dc7638e92cc746a8d8.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/54/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

54
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
	-H "Authorization: Bearer 7bfa4e744dfa3c2d8c017a957bab99f30218132445a0ed9c2797292c12923b38"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/52/flashcards
Content-Type: application/json
Authorization: Bearer 94e8afbb187cde18374c3b951924c50bc105830a1076e0e0b465cb600e2771bb
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 322,
      "chapter_id": 52,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:36.011Z",
      "created_at": "2016-09-01T13:38:36.011Z",
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 322,
      "chapter_id": 52,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:36.030Z",
      "created_at": "2016-09-01T13:38:36.030Z",
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
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 322,
      "chapter_id": 52,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:36.050Z",
      "created_at": "2016-09-01T13:38:36.050Z",
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
curl "api.goskive.com/v2/chapters/52/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94e8afbb187cde18374c3b951924c50bc105830a1076e0e0b465cb600e2771bb"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/114/questions
Content-Type: application/json
Authorization: Bearer be7bf068255741914ddbe09a52dece0c60fce749f0f02fcb98e6d735572b57ec
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":114,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 85,
    "obfuscated_id": "xR5KgQjIo2Y",
    "author_id": 569,
    "chapter_id": 114,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:54.145Z",
    "created_at": "2016-09-01T13:38:54.145Z",
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
        "id": 170,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 171,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 172,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 173,
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
curl "api.goskive.com/v2/chapters/114/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":114,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be7bf068255741914ddbe09a52dece0c60fce749f0f02fcb98e6d735572b57ec"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/113/questions
Content-Type: application/json
Authorization: Bearer 441547a70617ab64b5f0fcec66552f60e1a6b3cf2c358b1672aa8a9aaecfe953
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":113,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 84,
    "obfuscated_id": "Hu6DTUHzhWo",
    "author_id": 566,
    "chapter_id": 113,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:53.926Z",
    "created_at": "2016-09-01T13:38:53.926Z",
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
        "id": 168,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 169,
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
curl "api.goskive.com/v2/chapters/113/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":113,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 441547a70617ab64b5f0fcec66552f60e1a6b3cf2c358b1672aa8a9aaecfe953"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/116/questions
Content-Type: application/json
Authorization: Bearer 014245896a43eba9e7c61f49cabadfc5deb2d49d2bcfebfa8bd540e79b893a63
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 87,
    "obfuscated_id": "Jisk1d9Nmeo",
    "author_id": 575,
    "chapter_id": 116,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:54.649Z",
    "created_at": "2016-09-01T13:38:54.649Z",
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
        "id": 177,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 178,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/116/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 014245896a43eba9e7c61f49cabadfc5deb2d49d2bcfebfa8bd540e79b893a63"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/115/questions
Content-Type: application/json
Authorization: Bearer 505f68183b8029918113c2ff1326aa15f5081ca08b710889327587c9a5ddb48c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":115,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 86,
    "obfuscated_id": "7q-2LHZR3Kk",
    "author_id": 572,
    "chapter_id": 115,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:54.410Z",
    "created_at": "2016-09-01T13:38:54.410Z",
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
        "id": 174,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 175,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 176,
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
curl "api.goskive.com/v2/chapters/115/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":115,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 505f68183b8029918113c2ff1326aa15f5081ca08b710889327587c9a5ddb48c"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/117/questions
Content-Type: application/json
Authorization: Bearer 039b96fd58490830d1de40974ba96917d164e475e9631497a7d48267618eb593
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 578,
      "chapter_id": 117,
      "position": 75,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:54.864Z",
      "created_at": "2016-09-01T13:38:54.838Z",
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
    },
    {
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 579,
      "chapter_id": 117,
      "position": 76,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:54.928Z",
      "created_at": "2016-09-01T13:38:54.901Z",
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
          "id": 181,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 182,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 580,
      "chapter_id": 117,
      "position": 77,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:54.993Z",
      "created_at": "2016-09-01T13:38:54.966Z",
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
          "id": 183,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 184,
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
curl "api.goskive.com/v2/chapters/117/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 039b96fd58490830d1de40974ba96917d164e475e9631497a7d48267618eb593"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/156
Content-Type: application/json
Authorization: Bearer db34515395e4dfe1a3b11e12f3ab40188d44945c4c24712e8eff6642d00723c1
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
curl "api.goskive.com/v2/chapters/156" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db34515395e4dfe1a3b11e12f3ab40188d44945c4c24712e8eff6642d00723c1"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/157
Content-Type: application/json
Authorization: Bearer 5e01ecc217d8d2e679b8ff590b3c57c8b00a3cfa6bcbc70411226cc339a0804a
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
curl "api.goskive.com/v2/chapters/157" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e01ecc217d8d2e679b8ff590b3c57c8b00a3cfa6bcbc70411226cc339a0804a"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/154
Content-Type: application/json
Authorization: Bearer d95b523b3782e8a5b63237e3391f9ab757ad55929edd18ba41c0e07cd3ad777b
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
curl "api.goskive.com/v2/chapters/154" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d95b523b3782e8a5b63237e3391f9ab757ad55929edd18ba41c0e07cd3ad777b"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/158
Content-Type: application/json
Authorization: Bearer 9ae2ff7f11e4dda6b6c101cd7f6468da2d618f0651f44aa2b9ba111700ef7612
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/158" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ae2ff7f11e4dda6b6c101cd7f6468da2d618f0651f44aa2b9ba111700ef7612"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/150
Content-Type: application/json
Authorization: Bearer f5f40c9f66969f0d53fff7690ec2517699906773c5cc26ed172ca68f0a9154de
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
    "id": 150,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-01T13:39:03.987Z",
    "course_id": 247,
    "author_id": 741,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 745,
        "chapter_id": 150,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-09-01T13:39:03.982Z",
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
        "id": 111,
        "obfuscated_id": "G-D-sgMUtTw",
        "author_id": 743,
        "chapter_id": 150,
        "position": 98,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-09-01T13:39:03.878Z",
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
            "id": 225,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 226,
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
curl "api.goskive.com/v2/chapters/150" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5f40c9f66969f0d53fff7690ec2517699906773c5cc26ed172ca68f0a9154de"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/152
Content-Type: application/json
Authorization: Bearer e664c0c6dc0c6f2cc0c2783ecb95dea8f47a7c70dff0ec375f979e9753945da5
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
    "id": 152,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-01T13:39:04.591Z",
    "course_id": 249,
    "author_id": 755,
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
curl "api.goskive.com/v2/chapters/152" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e664c0c6dc0c6f2cc0c2783ecb95dea8f47a7c70dff0ec375f979e9753945da5"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 8d715f13ac6fe30c2542554e04a114ef92550218115eca452fb477d93c88a030
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
    "id": 59,
    "author_id": 892,
    "reply_to_id": 58,
    "created_at": "2016-09-01T13:39:12.419Z",
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
curl "api.goskive.com/v2/comments/58/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d715f13ac6fe30c2542554e04a114ef92550218115eca452fb477d93c88a030"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer d6e3ab5e8838914d1268803b2ab91d416ebfecf4738cabf568b67df2cadd0248
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
curl "api.goskive.com/v2/comments/60/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6e3ab5e8838914d1268803b2ab91d416ebfecf4738cabf568b67df2cadd0248"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/1
Content-Type: application/json
Authorization: Bearer 807922e9a2fc602342851b114e5a0a2dae062717fa93e92879af5591a54c4e04
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
curl "api.goskive.com/v2/comments/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 807922e9a2fc602342851b114e5a0a2dae062717fa93e92879af5591a54c4e04"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/40/republish
Content-Type: application/json
Authorization: Bearer 3dea97d50073bd1c9b1a99e8347afa4c5b3a015922b5719c35ffda4ae20d4a56
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
curl "api.goskive.com/v2/comments/40/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3dea97d50073bd1c9b1a99e8347afa4c5b3a015922b5719c35ffda4ae20d4a56"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer a0c742cc5723bf51cd8499fbd376d0d568fd0d8964e75e3b4b408b2eddc3a684
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0c742cc5723bf51cd8499fbd376d0d568fd0d8964e75e3b4b408b2eddc3a684"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/39/report
Content-Type: application/json
Authorization: Bearer ef556d7432fdf659f9b580ccbbc3e8f31b9163339d4844409f3b01fca6af8d2b
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/39/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef556d7432fdf659f9b580ccbbc3e8f31b9163339d4844409f3b01fca6af8d2b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer 6197546f6d746b2f7be89a14bc3b9fae1e2adfcbd9243c8606118ea81b7c208d
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
    "id": 4,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-09-01T13:38:14.195Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6197546f6d746b2f7be89a14bc3b9fae1e2adfcbd9243c8606118ea81b7c208d"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 52f60df38325547a24ac2c1b26db6385298bd2ea5413ec6d0358bf7b23c51783
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
      "id": 1,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-01T13:38:14.130Z"
    },
    {
      "id": 2,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-01T13:38:14.135Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-01T13:38:14.139Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52f60df38325547a24ac2c1b26db6385298bd2ea5413ec6d0358bf7b23c51783"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 76781dd4d23c8accf77eca6b1f9c80ba5783c89f642bf6175e3d21241de0db3b
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
      "id": 11,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/6557160cf523e6b44ee9eac06061463b0fcbd3b1.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/f4961300e395cd3802066da84ade8e1cdd20826f.png",
      "widgets": [

      ]
    },
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
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76781dd4d23c8accf77eca6b1f9c80ba5783c89f642bf6175e3d21241de0db3b"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/28/company_profiles
Content-Type: application/json
Authorization: Bearer 09206f3a7aa2e7ccd4e633a3f653aa36dcb792c6cacef9e3e17117d2921c3551
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
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9d765d9b895a77cd295c7f5e57af933f977bb87f.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/648481f5d8c76852bca2fea2b305e3b694878255.png",
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
curl "api.goskive.com/v2/companies/28/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09206f3a7aa2e7ccd4e633a3f653aa36dcb792c6cacef9e3e17117d2921c3551"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer ba61a5481cd9db4b8b19b884c6bee0a92c5519bf7e0714245589b684a903f020
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 5,
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
      "id": 4,
      "title": "Campaign 4",
      "company_id": 8,
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
	-H "Authorization: Bearer ba61a5481cd9db4b8b19b884c6bee0a92c5519bf7e0714245589b684a903f020"
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
Authorization: Bearer 481dcdda6fbc9a8b3e6e7639a2310b5958763f9e7226d31f3571a09c42242e25
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
	-H "Authorization: Bearer 481dcdda6fbc9a8b3e6e7639a2310b5958763f9e7226d31f3571a09c42242e25"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1c00ed166cd349a6ee2002f3ad94f846c919d9fa4b9d6608a53b0234dab187cf
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
    "id": 79,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-01T13:38:46.455Z",
    "course_id": 149,
    "author_id": 455,
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
	-H "Authorization: Bearer 1c00ed166cd349a6ee2002f3ad94f846c919d9fa4b9d6608a53b0234dab187cf"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5947c4f2fee4673882399eec0363d855a74d8bd3656bcceed6147b917e02d4ab
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
      "id": 83,
      "title": "Clever Chapter Title 75",
      "position": 1,
      "updated_at": "2016-09-01T13:38:46.975Z",
      "course_id": 152,
      "author_id": 464,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 84,
      "title": "Clever Chapter Title 76",
      "position": 2,
      "updated_at": "2016-09-01T13:38:46.999Z",
      "course_id": 152,
      "author_id": 465,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 85,
      "title": "Clever Chapter Title 77",
      "position": 3,
      "updated_at": "2016-09-01T13:38:47.134Z",
      "course_id": 152,
      "author_id": 466,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-09-01T13:38:47.121Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5947c4f2fee4673882399eec0363d855a74d8bd3656bcceed6147b917e02d4ab"
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
      "id": 89,
      "title": "Clever Chapter Title 81",
      "position": 1,
      "updated_at": "2016-09-01T13:38:47.674Z",
      "course_id": 155,
      "author_id": 478,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 90,
      "title": "Clever Chapter Title 82",
      "position": 2,
      "updated_at": "2016-09-01T13:38:47.698Z",
      "course_id": 155,
      "author_id": 479,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 91,
      "title": "Clever Chapter Title 83",
      "position": 3,
      "updated_at": "2016-09-01T13:38:47.824Z",
      "course_id": 155,
      "author_id": 480,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-09-01T13:38:47.814Z",
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
Authorization: Bearer a8e09ff7a7acdfab8dcab019ea7f96c316dfdcc456c6833f65799081801b7360
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
      "id": 86,
      "title": "Clever Chapter Title 78",
      "position": 1,
      "updated_at": "2016-09-01T13:38:47.338Z",
      "course_id": 153,
      "author_id": 471,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 87,
      "title": "Clever Chapter Title 79",
      "position": 2,
      "updated_at": "2016-09-01T13:38:47.362Z",
      "course_id": 153,
      "author_id": 472,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 88,
      "title": "Clever Chapter Title 80",
      "position": 3,
      "updated_at": "2016-09-01T13:38:47.386Z",
      "course_id": 153,
      "author_id": 473,
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
	-H "Authorization: Bearer a8e09ff7a7acdfab8dcab019ea7f96c316dfdcc456c6833f65799081801b7360"
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
      "id": 92,
      "title": "Clever Chapter Title 84",
      "position": 1,
      "updated_at": "2016-09-01T13:38:48.036Z",
      "course_id": 157,
      "author_id": 485,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 93,
      "title": "Clever Chapter Title 85",
      "position": 2,
      "updated_at": "2016-09-01T13:38:48.061Z",
      "course_id": 157,
      "author_id": 486,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 94,
      "title": "Clever Chapter Title 86",
      "position": 3,
      "updated_at": "2016-09-01T13:38:48.086Z",
      "course_id": 157,
      "author_id": 487,
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
Authorization: Bearer a0b9e9c8b0dd25745d6a1a5444798dee3a0b8280d883bb183e4accf69f3f4475
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
    "id": 2,
    "course_id": 286,
    "user_id": 873,
    "updated_at": "2016-09-01T13:39:11.428Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0b9e9c8b0dd25745d6a1a5444798dee3a0b8280d883bb183e4accf69f3f4475"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 6ef0d5b7e8d761ba77356b9e3773a95667bd51e804727138a778f17a70c816a6
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
      "course_id": 290,
      "user_id": 883,
      "updated_at": "2016-09-01T13:39:11.966Z"
    },
    {
      "id": 7,
      "course_id": 290,
      "user_id": 884,
      "updated_at": "2016-09-01T13:39:11.984Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ef0d5b7e8d761ba77356b9e3773a95667bd51e804727138a778f17a70c816a6"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer b7943e3ffc9548e2425c3db18db2c974f13b403b48eed72fbe8f28a5d8fe9403
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
	-H "Authorization: Bearer b7943e3ffc9548e2425c3db18db2c974f13b403b48eed72fbe8f28a5d8fe9403"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9b93cc174918c8d2f89bbd1b2b09d631e45cbc704c01f8b29d691b852e9f8733
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
	-H "Authorization: Bearer 9b93cc174918c8d2f89bbd1b2b09d631e45cbc704c01f8b29d691b852e9f8733"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8baea0c9baa78d10f82f0b3393f446836c928985001e566410bd4eb2b1685cce
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
	-H "Authorization: Bearer 8baea0c9baa78d10f82f0b3393f446836c928985001e566410bd4eb2b1685cce"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b864d6f92c43172582dad5092d2c59f2de7faa5d24a81d54aab9cb54f43024e6
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
	-H "Authorization: Bearer b864d6f92c43172582dad5092d2c59f2de7faa5d24a81d54aab9cb54f43024e6"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ee5aab39a913a98c3be60492ffd7e1daca56aedb3315bb14f150b2c3c07162c9
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
	-H "Authorization: Bearer ee5aab39a913a98c3be60492ffd7e1daca56aedb3315bb14f150b2c3c07162c9"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer a1a148305fb1b7f93ae20fb04ffb5a25eab28adab34d4aff77c8bed69c0f6c85
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
    "creator_id": 291,
    "id": 103,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 108,
    "additional_university_ids": [

    ],
    "topic_id": 106,
    "discipline_id": 106,
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
    "chapters_updated_at": "2016-09-01T13:38:33.069Z",
    "updated_at": "2016-09-01T13:38:33.072Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 46,
        "title": "Clever Chapter Title 46",
        "position": 1,
        "updated_at": "2016-09-01T13:38:33.040Z",
        "course_id": 103,
        "author_id": 291,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-01T13:38:32.963Z",
        "questions_updated_at": "2016-09-01T13:38:32.655Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 47,
        "title": "Clever Chapter Title 47",
        "position": 2,
        "updated_at": "2016-09-01T13:38:33.069Z",
        "course_id": 103,
        "author_id": 291,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-01T13:38:33.007Z",
        "questions_updated_at": "2016-09-01T13:38:32.784Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 292,
        "chapter_id": 46,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.940Z",
        "created_at": "2016-09-01T13:38:32.940Z",
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
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 292,
        "chapter_id": 47,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.983Z",
        "created_at": "2016-09-01T13:38:32.983Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 292,
        "chapter_id": 46,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.963Z",
        "created_at": "2016-09-01T13:38:32.963Z",
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
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 292,
        "chapter_id": 47,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:33.007Z",
        "created_at": "2016-09-01T13:38:33.007Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 292,
        "chapter_id": 46,
        "position": 39,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.597Z",
        "created_at": "2016-09-01T13:38:32.571Z",
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
            "id": 96,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 97,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 292,
        "chapter_id": 46,
        "position": 40,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.655Z",
        "created_at": "2016-09-01T13:38:32.630Z",
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
            "id": 98,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 99,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 292,
        "chapter_id": 47,
        "position": 41,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.725Z",
        "created_at": "2016-09-01T13:38:32.698Z",
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
            "id": 100,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 101,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 292,
        "chapter_id": 47,
        "position": 42,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:32.784Z",
        "created_at": "2016-09-01T13:38:32.759Z",
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
            "id": 102,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 103,
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
	-H "Authorization: Bearer a1a148305fb1b7f93ae20fb04ffb5a25eab28adab34d4aff77c8bed69c0f6c85"
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
    "creator_id": 297,
    "id": 104,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 109,
    "additional_university_ids": [

    ],
    "topic_id": 107,
    "discipline_id": 107,
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
    "chapters_updated_at": "2016-09-01T13:38:33.809Z",
    "updated_at": "2016-09-01T13:38:33.812Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 48,
        "title": "Clever Chapter Title 48",
        "position": 1,
        "updated_at": "2016-09-01T13:38:33.778Z",
        "course_id": 104,
        "author_id": 297,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-01T13:38:33.673Z",
        "questions_updated_at": "2016-09-01T13:38:33.329Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 49,
        "title": "Clever Chapter Title 49",
        "position": 2,
        "updated_at": "2016-09-01T13:38:33.809Z",
        "course_id": 104,
        "author_id": 297,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-01T13:38:33.718Z",
        "questions_updated_at": "2016-09-01T13:38:33.459Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 297,
        "chapter_id": 48,
        "position": 45,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:33.329Z",
        "created_at": "2016-09-01T13:38:33.303Z",
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
            "id": 108,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 109,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 297,
        "chapter_id": 49,
        "position": 47,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:33.459Z",
        "created_at": "2016-09-01T13:38:33.433Z",
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
            "id": 112,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 113,
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
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/106/pin
Content-Type: application/json
Authorization: Bearer 023d8f288faa65f832003d98fe3f10dbd89736aa27c6d3f53cdf2fb189d0c67d
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/106/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 023d8f288faa65f832003d98fe3f10dbd89736aa27c6d3f53cdf2fb189d0c67d"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/101/pin
Content-Type: application/json
Authorization: Bearer 9260741da52a3c15d278c9456f6df6cffeb91bb4f713aea93f0a6c3582c199b8
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/101/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9260741da52a3c15d278c9456f6df6cffeb91bb4f713aea93f0a6c3582c199b8"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c5875ffb47a5e08d18d21bd60c5d8757b894c31d65b14c328d2907e0cf712963
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
    "creator_id": 314,
    "id": 109,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 114,
    "additional_university_ids": [

    ],
    "topic_id": 112,
    "discipline_id": 112,
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
    "updated_at": "2016-09-01T13:38:35.197Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5875ffb47a5e08d18d21bd60c5d8757b894c31d65b14c328d2907e0cf712963"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 591787190a4e82ca97138699d37a920b2f2191a32f2683784f253a1f8dd437c2
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
    "id": 402,
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
    "created_at": "2016-09-01T13:38:42.287Z",
    "updated_at": "2016-09-01T13:38:42.287Z",
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
	-H "Authorization: Bearer 591787190a4e82ca97138699d37a920b2f2191a32f2683784f253a1f8dd437c2"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 6df1108fa23ffe283752c976e4a594517cf3da1653715a5021b69db53bc25d0a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[142]}
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
    "id": 398,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      142
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-01T13:38:41.972Z",
    "updated_at": "2016-09-01T13:38:42.017Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[142]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6df1108fa23ffe283752c976e4a594517cf3da1653715a5021b69db53bc25d0a"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 5905e50213167eb3bb9035208b8f2fec976d801178c8375273a0ecca3772d8f8
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
    "id": 399,
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
    "created_at": "2016-09-01T13:38:42.040Z",
    "updated_at": "2016-09-01T13:38:42.040Z",
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
	-H "Authorization: Bearer 5905e50213167eb3bb9035208b8f2fec976d801178c8375273a0ecca3772d8f8"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 00d3d10a0fd008aefa95c4ab3ad1069854a7e4b766d50662bcbdfec53241f175
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[144]}
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
    "id": 400,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      144
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-01T13:38:42.146Z",
    "updated_at": "2016-09-01T13:38:42.146Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[144]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00d3d10a0fd008aefa95c4ab3ad1069854a7e4b766d50662bcbdfec53241f175"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 2b999fe2c52ba277f3267a886fc57a59506f2dce2780aaece0fc1f43a69f7acf
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

141
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
    "id": 397,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/b191c723e16619afd55c1c2ac3ee7fbf488311b8.jpg",
    "university_id": null,
    "fields_of_study": [
      141
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-01T13:38:41.504Z",
    "updated_at": "2016-09-01T13:38:41.908Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/a9a0d529fd6f22489674ae605b27089ae27ca0dd.jpg",
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

141
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 2b999fe2c52ba277f3267a886fc57a59506f2dce2780aaece0fc1f43a69f7acf"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer bbf992837768aa1a96bce0b63410d9022649c56b8a416e490a892ed4d6a59842
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
      "id": 1,
      "bookmarkable_id": 4,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 5,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 6,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbf992837768aa1a96bce0b63410d9022649c56b8a416e490a892ed4d6a59842"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 655df34e9dea33121018c9cda8da2b11cb38a8e7607c886baadb0d6139cddcf3
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
      "id": 9,
      "title": "Campaign 9",
      "company_id": 17,
      "precluded_campaign_ids": [

      ],
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
      "id": 10,
      "title": "Campaign 10",
      "company_id": 18,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
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
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/e454a32c998f7d7ac27f091147bbb511cdb6f8e8.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/0d72c01d65a8bf6733c1fdf8c672243b6d546a9e.png",
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
	-H "Authorization: Bearer 655df34e9dea33121018c9cda8da2b11cb38a8e7607c886baadb0d6139cddcf3"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer ed7cad7a4cb75125af522672674386e0725938db8037d750a1cc77e17a6a2530
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
      "creator_id": 339,
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-92",
      "html_url": "https://goskive.com/course/mit-course-92",
      "slug": "mit-course-92",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 123,
      "discipline_id": 123,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 92",
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
      "updated_at": "2016-09-01T13:38:37.807Z",
      "shortname": "mit-course-92"
    },
    {
      "creator_id": 340,
      "id": 121,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-93",
      "html_url": "https://goskive.com/course/mit-course-93",
      "slug": "mit-course-93",
      "university_id": 127,
      "additional_university_ids": [

      ],
      "topic_id": 124,
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
      "updated_at": "2016-09-01T13:38:37.894Z",
      "shortname": "mit-course-93"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed7cad7a4cb75125af522672674386e0725938db8037d750a1cc77e17a6a2530"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a6595d4dec445b74da9d0b0a3129c25a75d74789c0fef1a7698ea4ef87b2a333
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-09-01T13:38:55.517Z"
      },
      "created_at": "2016-09-01T13:38:55.523Z",
      "updated_at": "2016-09-01T13:38:55.523Z"
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-09-01T13:38:55.517Z"
      },
      "created_at": "2016-09-01T13:38:55.523Z",
      "updated_at": "2016-09-01T13:38:55.523Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6595d4dec445b74da9d0b0a3129c25a75d74789c0fef1a7698ea4ef87b2a333"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 43ab3bfb61323bb62e8fbde9057fe383690163468008af99f763ee25302bcbed
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
      "id": 8,
      "created_at": "2016-09-01T13:38:39.984Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 48,
      "updated_at": "2016-09-01T13:38:40.118Z",
      "author_id": "367",
      "thread_subject_id": "129",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 9,
      "created_at": "2016-09-01T13:38:40.103Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 49,
      "updated_at": "2016-09-01T13:38:40.123Z",
      "author_id": "370",
      "thread_subject_id": "130",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-09-01T13:38:40.343Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 6,
      "updated_at": "2016-09-01T13:38:40.343Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-09-01T13:38:40.538Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-09-01T13:38:40.538Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 12,
      "created_at": "2016-09-01T13:38:40.741Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-09-01T13:38:40.741Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 13,
      "created_at": "2016-09-01T13:38:40.908Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 74,
      "updated_at": "2016-09-01T13:38:40.908Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-09-01T13:38:41.087Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 75,
      "updated_at": "2016-09-01T13:38:41.087Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-09-01T13:38:41.268Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 76,
      "updated_at": "2016-09-01T13:38:41.268Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43ab3bfb61323bb62e8fbde9057fe383690163468008af99f763ee25302bcbed"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/16
Content-Type: application/json
Authorization: Bearer 8b91ff97a03dc43db24db6f017adebe24f1e5196ba539a90e7f5e622919850e3
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-09-01T13:28:41.000Z"}}
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
    "id": 16,
    "created_at": "2016-09-01T13:38:41.420Z",
    "read_at": "2016-09-01T13:28:41.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 50,
    "updated_at": "2016-09-01T13:38:41.464Z",
    "author_id": "395",
    "thread_subject_id": "137",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/16" -d '{"notification":{"read_at":"2016-09-01T13:28:41.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b91ff97a03dc43db24db6f017adebe24f1e5196ba539a90e7f5e622919850e3"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 579153ad9cbf2a09ed0c4b6aa41eb2eac802a424e7f0a32757deef8c5368cd1f
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
      "course_id": 16,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-01T13:38:18.206Z",
      "course_published": true,
      "updated_at": "2016-09-01T13:38:18.198Z"
    },
    {
      "id": 5,
      "course_id": 17,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-01T13:38:18.293Z",
      "course_published": true,
      "updated_at": "2016-09-01T13:38:18.285Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 579153ad9cbf2a09ed0c4b6aa41eb2eac802a424e7f0a32757deef8c5368cd1f"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer a6268e9126e6a3458d98d69868be33727854d5ff46308d5c2e87e20675ed7c14
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
    "id": 2,
    "course_id": 13,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-01T13:38:17.774Z",
    "course_published": true,
    "updated_at": "2016-09-01T13:38:17.766Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6268e9126e6a3458d98d69868be33727854d5ff46308d5c2e87e20675ed7c14"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer dc3cdc08003462f015a0db9ba0cae7bffaaffab661eacc57a6e5e9a8276ca9ef
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
    "id": 1,
    "course_id": 12,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-09-01T13:38:17.658Z",
    "course_published": true,
    "updated_at": "2016-09-01T13:38:17.650Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc3cdc08003462f015a0db9ba0cae7bffaaffab661eacc57a6e5e9a8276ca9ef"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 87938a3779020729beb157ebca8b7bfe53d00a4c3c95f77fc12df67f8e775649
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
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 116,
      "user_id": 775
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 117,
      "user_id": 775
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 118,
      "user_id": 775
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 119,
      "user_id": 775
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87938a3779020729beb157ebca8b7bfe53d00a4c3c95f77fc12df67f8e775649"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/257
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
    "id": 257,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 257,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 257
      },
      {
        "id": 258,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 257
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/257" -X GET \
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
      "id": 258,
      "name": "Optimized homogeneous migration",
      "name_translations": {
        "en": "Optimized homogeneous migration"
      }
    },
    {
      "id": 259,
      "name": "Streamlined 4th generation benchmark",
      "name_translations": {
        "en": "Streamlined 4th generation benchmark"
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
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer 7e2c8e6271092a04ca4b48312bf13896433b827e1d8bcf7d298737fe291282d5
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
    "id": 20,
    "user_id": 598,
    "feedbackable_id": 55,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-09-01T13:38:56.210Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e2c8e6271092a04ca4b48312bf13896433b827e1d8bcf7d298737fe291282d5"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/fix
Content-Type: application/json
Authorization: Bearer e3b89c3f7af76fdd5041d668f3d867d3d99fbcb2c9609577d11929f04287c3a2
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
    "id": 46,
    "user_id": 716,
    "feedbackable_id": 62,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-09-01T13:39:01.602Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/46/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3b89c3f7af76fdd5041d668f3d867d3d99fbcb2c9609577d11929f04287c3a2"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/22
Content-Type: application/json
Authorization: Bearer 1df70be4a84a42c50ef42efdc6edb782aaad3902fe0b08bf4ca08e831a86b795
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
    "id": 22,
    "user_id": 608,
    "feedbackable_id": 57,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-01T13:38:56.698Z",
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
curl "api.goskive.com/v2/feedbacks/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1df70be4a84a42c50ef42efdc6edb782aaad3902fe0b08bf4ca08e831a86b795"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer 19013beff14c9166a17165797f63232ff468c4bfb32e6cfd76522338090d6ec9
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
curl "api.goskive.com/v2/feedbacks/21/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19013beff14c9166a17165797f63232ff468c4bfb32e6cfd76522338090d6ec9"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 9196af8f5d165e7e40877bfabcbbae863de56e04d83c8572c7b5bbd11891dbfa
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
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9196af8f5d165e7e40877bfabcbbae863de56e04d83c8572c7b5bbd11891dbfa"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/fix
Content-Type: application/json
Authorization: Bearer 424bea04b1523b175fc814e1b3c5838285a4ca0d7b33988e65d8022502d5e5c4
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
curl "api.goskive.com/v2/feedbacks/44/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 424bea04b1523b175fc814e1b3c5838285a4ca0d7b33988e65d8022502d5e5c4"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/23
Content-Type: application/json
Authorization: Bearer 4b694325489ec42d4d7a2e38530b9dcd30fc2125d22b3e1cb3b3450f8296ce44
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
    "id": 23,
    "user_id": 613,
    "feedbackable_id": 58,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-01T13:38:57.005Z",
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
curl "api.goskive.com/v2/feedbacks/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b694325489ec42d4d7a2e38530b9dcd30fc2125d22b3e1cb3b3450f8296ce44"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/48/comments
Content-Type: application/json
Authorization: Bearer c707e89abab0d93bb072f41b2e3ba0bdefaef2758143183466e3f9a4d8a77081
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
    "id": 56,
    "author_id": 513,
    "reply_to_id": null,
    "created_at": "2016-09-01T13:38:49.578Z",
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
curl "api.goskive.com/v2/flashcards/48/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c707e89abab0d93bb072f41b2e3ba0bdefaef2758143183466e3f9a4d8a77081"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/47/comments
Content-Type: application/json
Authorization: Bearer 39ec2586475ce2644e28f91765982e36db9515ab3c618308b255166784541a48
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
    "id": 55,
    "author_id": 510,
    "reply_to_id": null,
    "created_at": "2016-09-01T13:38:49.274Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 18,
      "user_id": 510,
      "feedbackable_id": 47,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:49.270Z",
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
curl "api.goskive.com/v2/flashcards/47/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39ec2586475ce2644e28f91765982e36db9515ab3c618308b255166784541a48"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/46/comments
Content-Type: application/json
Authorization: Bearer b4e0f0871fb2c861cd91ca33519b30ad85496a2948e6e813ab3bfc1f7a963b04
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
      "id": 54,
      "author_id": 509,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:49.043Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 508,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:49.024Z",
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
curl "api.goskive.com/v2/flashcards/46/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4e0f0871fb2c861cd91ca33519b30ad85496a2948e6e813ab3bfc1f7a963b04"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/49/comments
Content-Type: application/json
Authorization: Bearer 0ec32d781d74ad324fbb44165d22c6a465c9b517c2a18d7f0eddf4fb995300e7
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
curl "api.goskive.com/v2/flashcards/49/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ec32d781d74ad324fbb44165d22c6a465c9b517c2a18d7f0eddf4fb995300e7"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/34/feedbacks
Content-Type: application/json
Authorization: Bearer 191331b7e604d852f07221596ece245ec158b8bba9044db21433a7965deea6af
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
    "id": 10,
    "user_id": 404,
    "feedbackable_id": 34,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-01T13:38:42.562Z",
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
curl "api.goskive.com/v2/flashcards/34/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 191331b7e604d852f07221596ece245ec158b8bba9044db21433a7965deea6af"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/39/feedbacks
Content-Type: application/json
Authorization: Bearer 8c6db2ed4e7b6f127779cd6d2486c91637cf5570e6aa134ed1218b14f8bd726d
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
      "id": 15,
      "user_id": 431,
      "feedbackable_id": 39,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:43.769Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 430,
      "feedbackable_id": 39,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:43.755Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/39/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c6db2ed4e7b6f127779cd6d2486c91637cf5570e6aa134ed1218b14f8bd726d"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/65/votes
Content-Type: application/json
Authorization: Bearer 5389e651458ef1b401b9fe2e622f1e3035e25e4a7b88ffeaed276417a2a0c619
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
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 65,
      "user_id": 729
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 65,
      "user_id": 728
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 65,
      "user_id": 727
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/65/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5389e651458ef1b401b9fe2e622f1e3035e25e4a7b88ffeaed276417a2a0c619"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/75/republish
Content-Type: application/json
Authorization: Bearer fef80bb8acdd6512794d24d27ff06951f3bea08afac890d558a8a9a4d7f69e83
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
curl "api.goskive.com/v2/flashcards/75/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fef80bb8acdd6512794d24d27ff06951f3bea08afac890d558a8a9a4d7f69e83"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/95/bookmark
Content-Type: application/json
Authorization: Bearer 3bd95d4316a00085603743a1e85d5736284b6cd44a463cbf0678b576fd8d9ca1
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/95/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bd95d4316a00085603743a1e85d5736284b6cd44a463cbf0678b576fd8d9ca1"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/70
Content-Type: application/json
Authorization: Bearer 6dadfc77c061211b80b5b5c6c9219037a3488f662adbd6c9786a9501dfcdcaa7
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/70" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dadfc77c061211b80b5b5c6c9219037a3488f662adbd6c9786a9501dfcdcaa7"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/71/downvote
Content-Type: application/json
Authorization: Bearer 65e9c31084df222ec1c3234e31928a1e7b457d391d87de0350ecdfca8a06fd32
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/71/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65e9c31084df222ec1c3234e31928a1e7b457d391d87de0350ecdfca8a06fd32"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/93
Content-Type: application/json
Authorization: Bearer d090c7e2a812375f69af6dc41518d1049c23cf4b61df92b5a68d5cbcebd9f243
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
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 863,
    "chapter_id": 186,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:39:10.926Z",
    "created_at": "2016-09-01T13:39:10.926Z",
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
curl "api.goskive.com/v2/flashcards/93" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d090c7e2a812375f69af6dc41518d1049c23cf4b61df92b5a68d5cbcebd9f243"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/77/report
Content-Type: application/json
Authorization: Bearer 0336d809051eb6015be0cdb51a17079fe94cb1ce8649347009793f7f32edd000
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/77/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0336d809051eb6015be0cdb51a17079fe94cb1ce8649347009793f7f32edd000"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/94/bookmark
Content-Type: application/json
Authorization: Bearer 2027f9f2021025756254c28ec6e3b36ad8eff7c480f6b5d09e1c2ed2b3eb8780
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/94/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2027f9f2021025756254c28ec6e3b36ad8eff7c480f6b5d09e1c2ed2b3eb8780"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/72
Content-Type: application/json
Authorization: Bearer 2af88974ed45a8d24452af7c208f2149027569aeb1ea4636d55c35e93bab224a
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
    "id": 72,
    "obfuscated_id": "oqzxOzwzIgw",
    "author_id": 794,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:39:07.265Z",
    "created_at": "2016-09-01T13:39:06.921Z",
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
curl "api.goskive.com/v2/flashcards/72" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2af88974ed45a8d24452af7c208f2149027569aeb1ea4636d55c35e93bab224a"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/73
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 8072170433dbd581588c8effd2267fdc3efef6522827caeba47c7dae3b772bbf
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
    "id": 73,
    "obfuscated_id": "LJvjpBojvP0",
    "author_id": 797,
    "chapter_id": 166,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:39:07.745Z",
    "created_at": "2016-09-01T13:39:07.406Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/30b4b6d1c3a7eb23d1308fa1da123a78142fe416.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/35bdf8301106b0f45e69bc668673c7913f68d43b.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/30b4b6d1c3a7eb23d1308fa1da123a78142fe416.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/35bdf8301106b0f45e69bc668673c7913f68d43b.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/73" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
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
	-H "Authorization: Bearer 8072170433dbd581588c8effd2267fdc3efef6522827caeba47c7dae3b772bbf"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/76/upvote
Content-Type: application/json
Authorization: Bearer 66bc03fbd4ba2d475a45e84f1109921481e404b4602569b89f1e49e73020fea1
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66bc03fbd4ba2d475a45e84f1109921481e404b4602569b89f1e49e73020fea1"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/flashcards/images/cache/presign
Content-Type: application/json
Authorization: Bearer 53a638ae363d8beb521b856ee881fc905d13c2ab549fd314adc5e30a30d7bf34
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
    "key": "cache/0d1fd71fcc697abefd37d0d92e9fc650",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOS0wMVQxNDozOTowN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8wZDFmZDcxZmNjNjk3YWJlZmQzN2QwZDkyZTlmYzY1MCJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwOTAxL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDkwMVQxMzM5MDdaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160901/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160901T133907Z",
    "x-amz-signature": "a552192a842263c07164ad58538e6f7dc7f3f428c51db762369573eb1e7d1bd7"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/images/cache/presign" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53a638ae363d8beb521b856ee881fc905d13c2ab549fd314adc5e30a30d7bf34"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/5/sign_ups
Content-Type: application/json
Authorization: Bearer 494c5890e2b63b1ac402aad47bc3e9c5c9d967640c3bf8365c28dbe47bf1a276
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
    "id": 1,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/5/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 494c5890e2b63b1ac402aad47bc3e9c5c9d967640c3bf8365c28dbe47bf1a276"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/4/sign_ups
Content-Type: application/json
Authorization: Bearer 8279568894ed1c55116fdba6974a8a767c4df2dfaf95cb7eafe6385cbde26677
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
	-H "Authorization: Bearer 8279568894ed1c55116fdba6974a8a767c4df2dfaf95cb7eafe6385cbde26677"
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
{"password":{"reset_password_token":"bquEz264MLxh1NBNTjQ5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "created_at": "2016-09-01T13:39:17.554Z",
  "updated_at": "2016-09-01T13:39:17.695Z",
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
  "audit_id": 4805
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"bquEz264MLxh1NBNTjQ5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
{"password":{"reset_password_token":"gm8Jz1ZLycdS86d-qpNy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 903,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-09-01T13:39:18.537Z",
  "updated_at": "2016-09-01T13:39:19.383Z",
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
  "audit_id": 4808
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"gm8Jz1ZLycdS86d-qpNy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/68/comments
Content-Type: application/json
Authorization: Bearer d52a4c7eeb877c8ae13ae78a086ad9426eec2e6bd9d565b40ef101adca0183f9
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
    "id": 45,
    "author_id": 353,
    "reply_to_id": null,
    "created_at": "2016-09-01T13:38:39.197Z",
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
curl "api.goskive.com/v2/questions/68/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d52a4c7eeb877c8ae13ae78a086ad9426eec2e6bd9d565b40ef101adca0183f9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/66/comments
Content-Type: application/json
Authorization: Bearer fe57cfd827a7a1171ab5964cfbc504d57bdbc8a8e87ec85a09b2b27c35c4a999
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
    "id": 44,
    "author_id": 347,
    "reply_to_id": null,
    "created_at": "2016-09-01T13:38:38.661Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 347,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:38.658Z",
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
curl "api.goskive.com/v2/questions/66/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe57cfd827a7a1171ab5964cfbc504d57bdbc8a8e87ec85a09b2b27c35c4a999"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/70/comments
Content-Type: application/json
Authorization: Bearer 445e6def1be8047112d39bf56a67819a40c6fadfaba64b5fe1a94facda7e58b9
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
      "id": 47,
      "author_id": 363,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:39.741Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 362,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:39.722Z",
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
curl "api.goskive.com/v2/questions/70/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 445e6def1be8047112d39bf56a67819a40c6fadfaba64b5fe1a94facda7e58b9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/67/comments
Content-Type: application/json
Authorization: Bearer a45b49f5a30fad524e1db53da3fea42ccf089d2544df9378d1c26de1cb382ddf
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
curl "api.goskive.com/v2/questions/67/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a45b49f5a30fad524e1db53da3fea42ccf089d2544df9378d1c26de1cb382ddf"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/38/feedbacks
Content-Type: application/json
Authorization: Bearer 2e2fcd264254191fd250a4e9bb8280c071a413966351f0dcabb72721b6fcd9b5
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
    "id": 7,
    "user_id": 257,
    "feedbackable_id": 38,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-09-01T13:38:29.800Z",
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
curl "api.goskive.com/v2/questions/38/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e2fcd264254191fd250a4e9bb8280c071a413966351f0dcabb72721b6fcd9b5"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/37/feedbacks
Content-Type: application/json
Authorization: Bearer 37c03a10ad1e83af476fd82f66d06db09ee6e276ad59fb03de3ca72524a8e660
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
      "id": 6,
      "user_id": 256,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:29.575Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 255,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:29.562Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/37/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37c03a10ad1e83af476fd82f66d06db09ee6e276ad59fb03de3ca72524a8e660"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/122/votes
Content-Type: application/json
Authorization: Bearer 4080e9ce719636535637b75d7abca059d7055f368e7c23ccc6b885ba08a347f8
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
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 909
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 908
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 907
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/122/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4080e9ce719636535637b75d7abca059d7055f368e7c23ccc6b885ba08a347f8"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/10/republish
Content-Type: application/json
Authorization: Bearer 5e80236c4dc8c6e97c27cdad02f9032fbc7d1e297f912c578ac42d2bd3d8c86e
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
curl "api.goskive.com/v2/questions/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e80236c4dc8c6e97c27cdad02f9032fbc7d1e297f912c578ac42d2bd3d8c86e"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/9/bookmark
Content-Type: application/json
Authorization: Bearer 5b6c3b953dec49ea9a11d0daf62716c4b5e52f15ea1001bebbd34a25e0624872
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/9/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b6c3b953dec49ea9a11d0daf62716c4b5e52f15ea1001bebbd34a25e0624872"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/15
Content-Type: application/json
Authorization: Bearer 4286f97e877189037cf8bfd22f9d720d9de81cd01c1cf1c92d74845d9eeba490
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4286f97e877189037cf8bfd22f9d720d9de81cd01c1cf1c92d74845d9eeba490"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/16/downvote
Content-Type: application/json
Authorization: Bearer 4eebb6d0594fd9c63b237c5d9449de0ff2e858ab6f7b9e678c18b1ff2cb1dceb
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/16/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eebb6d0594fd9c63b237c5d9449de0ff2e858ab6f7b9e678c18b1ff2cb1dceb"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/8
Content-Type: application/json
Authorization: Bearer da53dfc826d9e23b35e3f050d928cddf458267d34205e4ba2b110b7cdf76e392
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 146,
    "chapter_id": 8,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:23.319Z",
    "created_at": "2016-09-01T13:38:23.295Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 15,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 16,
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
curl "api.goskive.com/v2/questions/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da53dfc826d9e23b35e3f050d928cddf458267d34205e4ba2b110b7cdf76e392"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/7/report
Content-Type: application/json
Authorization: Bearer ce6a2569603e65c054039b3de2b6ac76ede81c4e111658e659a130767bd00fb2
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/7/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce6a2569603e65c054039b3de2b6ac76ede81c4e111658e659a130767bd00fb2"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/14/bookmark
Content-Type: application/json
Authorization: Bearer 7857da2679f039aa83a574ad6b0efd0da29468227949270cca17cfa557b335c7
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/14/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7857da2679f039aa83a574ad6b0efd0da29468227949270cca17cfa557b335c7"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/13
Content-Type: application/json
Authorization: Bearer 96d583f132633c8b7cc5d9b0040c91b0b8aa44e0efb871801fbc5c1234b3ece6
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":13,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-01T13:38:24.422Z","updated_at":"2016-09-01T13:38:24.447Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":13,"author_id":161,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 161,
    "chapter_id": 13,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-01T13:38:24.520Z",
    "created_at": "2016-09-01T13:38:24.422Z",
    "tags": [
      {
        "id": 12,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 11,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>13, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-09-01T13:38:24.422Z\", \"updated_at\"=>\"2016-09-01T13:38:24.447Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>13, \"author_id\"=>161, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 27,
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
curl "api.goskive.com/v2/questions/13" -d '{"question":{"question":{"id":13,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-01T13:38:24.422Z","updated_at":"2016-09-01T13:38:24.447Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":13,"author_id":161,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96d583f132633c8b7cc5d9b0040c91b0b8aa44e0efb871801fbc5c1234b3ece6"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/12/upvote
Content-Type: application/json
Authorization: Bearer 38cc804108af8c2e148c56c7e5500bc4164b19f9e0b599a63bba3b02a663c7fd
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/12/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38cc804108af8c2e148c56c7e5500bc4164b19f9e0b599a63bba3b02a663c7fd"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer bab1c1090ce28756754ede8080f7e86d9b68350547852b4f935ab0faa6320e62
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
      "creator_id": 318,
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 115,
      "discipline_id": 115,
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
      "updated_at": "2016-09-01T13:38:35.550Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bab1c1090ce28756754ede8080f7e86d9b68350547852b4f935ab0faa6320e62"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 4dc9c537e2df53f2fe4e9a2bb241e3f904e4e6ca13bfed2b249fef194a150081
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
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-117",
      "html_url": "https://goskive.com/university/uni-117",
      "slug": "uni-117",
      "name": "National School of Pizza",
      "short_name": "Uni 117",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/18b3243e0496f81e57c0841ffc50d1ffea7771fc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8235339619085a5aaf31c8771d17b1288f8e8a68.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-01T13:38:35.753Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-116",
      "html_url": "https://goskive.com/university/uni-116",
      "slug": "uni-116",
      "name": "National School of Pastry",
      "short_name": "Uni 116",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/10c45072caa721987b05dfcb635cef9f53e6bb5b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/abe07e3df800339993de4e0db7bdc7e30ac9c4ff.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-01T13:38:35.736Z",
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
	-H "Authorization: Bearer 4dc9c537e2df53f2fe4e9a2bb241e3f904e4e6ca13bfed2b249fef194a150081"
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
      "id": 85,
      "name": "Visionary system-worthy moderator",
      "name_translations": {
        "en": "Visionary system-worthy moderator"
      },
      "discipline_id": 85
    },
    {
      "id": 86,
      "name": "Focused multi-tasking capability",
      "name_translations": {
        "en": "Focused multi-tasking capability"
      },
      "discipline_id": 86
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
GET /v2/topics/84
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
    "id": 84,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 84
  }
}
```



```shell
curl "api.goskive.com/v2/topics/84" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer a2d88d9767a13bff970faede14c2a1da27cf19c3540f362a7d2f1ec95a9f0f2c
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
      "id": 84,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-84",
      "html_url": "https://goskive.com/university/uni-84",
      "slug": "uni-84",
      "name": "University 80",
      "short_name": "Uni 84",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/007ac229263210b73c1c1b94495f61eba41fa753.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/02bc84a61eeca0d671b84f4cda55974ecc3b4877.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-01T13:38:28.057Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-85",
      "html_url": "https://goskive.com/university/uni-85",
      "slug": "uni-85",
      "name": "University 81",
      "short_name": "Uni 85",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b2a0a8b1306563d6a7102405ac5059dfd1ced439.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/0e64cc97b5989d48b0a4bbc801464a26f5eda68b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-01T13:38:28.072Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 86,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-86",
      "html_url": "https://goskive.com/university/uni-86",
      "slug": "uni-86",
      "name": "University 82",
      "short_name": "Uni 86",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b93ec4e030cd802e8eca31375c185e60bad55d8a.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ef152e162154145674c69af773a9f28789c3e75e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-01T13:38:28.087Z",
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
	-H "Authorization: Bearer a2d88d9767a13bff970faede14c2a1da27cf19c3540f362a7d2f1ec95a9f0f2c"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer cd86b2bdfb1f21df13b8709d9e4a50cf8dd357eb59741f1e4d9f3f9f8f463fd5
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
    "id": 87,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9451ed8e9606506be831ef3f1de113d07d668ac4.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c11ef0898fe214641029ad9e3df223926cc45bcb.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-09-01T13:38:28.168Z",
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
	-H "Authorization: Bearer cd86b2bdfb1f21df13b8709d9e4a50cf8dd357eb59741f1e4d9f3f9f8f463fd5"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c4b4bf1569652a76ff1816af183c5a718af74aab089af486cccb2efe2fac5ff4
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":212,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 562,
    "id": 204,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 188,
    "additional_university_ids": [

    ],
    "topic_id": 212,
    "discipline_id": 212,
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
    "chapters_updated_at": "2016-09-01T13:38:53.573Z",
    "updated_at": "2016-09-01T13:38:53.580Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 110,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-09-01T13:38:53.545Z",
        "course_id": 204,
        "author_id": 562,
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
        "id": 111,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-09-01T13:38:53.560Z",
        "course_id": 204,
        "author_id": 562,
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
        "id": 112,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-09-01T13:38:53.573Z",
        "course_id": 204,
        "author_id": 562,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":212,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4b4bf1569652a76ff1816af183c5a718af74aab089af486cccb2efe2fac5ff4"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2bc6bb2d64769bdd5082017759e071d408c172965ff2bc96682f43bd75a0a5fd
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":213,"published":false}}
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
    "creator_id": 563,
    "id": 205,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 189,
    "additional_university_ids": [

    ],
    "topic_id": 213,
    "discipline_id": 213,
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
    "updated_at": "2016-09-01T13:38:53.749Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":213,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bc6bb2d64769bdd5082017759e071d408c172965ff2bc96682f43bd75a0a5fd"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 310b8d2866c91728b75d2b0420755c11deebafb9e0f94c1d6fb49c40224fd136
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
      "creator_id": 530,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-133",
      "html_url": "https://goskive.com/course/fu-course-133",
      "slug": "fu-course-133",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "topic_id": 184,
      "discipline_id": 184,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 133",
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
      "updated_at": "2016-09-01T13:38:50.792Z",
      "shortname": "fu-course-133"
    },
    {
      "creator_id": 530,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
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
      "chapters_updated_at": "2016-09-01T13:38:50.958Z",
      "updated_at": "2016-09-01T13:38:50.960Z",
      "shortname": "fu-course-134"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 310b8d2866c91728b75d2b0420755c11deebafb9e0f94c1d6fb49c40224fd136"
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
      "creator_id": 540,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "topic_id": 192,
      "discipline_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
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
      "updated_at": "2016-09-01T13:38:51.565Z",
      "shortname": "fu-course-141"
    },
    {
      "creator_id": 540,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "topic_id": 193,
      "discipline_id": 193,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "chapters_updated_at": "2016-09-01T13:38:51.727Z",
      "updated_at": "2016-09-01T13:38:51.729Z",
      "shortname": "fu-course-142"
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
Authorization: Bearer ffaace4a3731b67c5433e8a0e6210b52e5d7ff8638f4db05d96e213cc4cffea0
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
      "creator_id": 536,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 176,
      "additional_university_ids": [

      ],
      "topic_id": 188,
      "discipline_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
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
      "updated_at": "2016-09-01T13:38:51.221Z",
      "shortname": "fu-course-137"
    },
    {
      "creator_id": 536,
      "id": 181,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 176,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 189,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
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
      "updated_at": "2016-09-01T13:38:51.263Z",
      "shortname": "fu-course-138"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffaace4a3731b67c5433e8a0e6210b52e5d7ff8638f4db05d96e213cc4cffea0"
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
      "creator_id": 545,
      "id": 188,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "topic_id": 196,
      "discipline_id": 196,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
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
      "updated_at": "2016-09-01T13:38:51.954Z",
      "shortname": "fu-course-145"
    },
    {
      "creator_id": 545,
      "id": 189,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "topic_id": 197,
      "discipline_id": 197,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
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
      "updated_at": "2016-09-01T13:38:51.995Z",
      "shortname": "fu-course-146"
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
Authorization: Bearer c69545ee9dfc068ffd6d6a6c0b08c266a9160247bb37ab9541872123384c21d4
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
  "id": 6,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-09-01T13:38:14.669Z",
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
	-H "Authorization: Bearer c69545ee9dfc068ffd6d6a6c0b08c266a9160247bb37ab9541872123384c21d4"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/732
Content-Type: application/json
Authorization: Bearer d767084b84c338d45bb744462fc5b7f49e2f149d76dd46830321c5b358b4244e
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
    "id": 732,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 231,
    "fields_of_study": [
      255,
      256
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-09-01T13:39:02.612Z",
    "updated_at": "2016-09-01T13:39:02.612Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/732" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d767084b84c338d45bb744462fc5b7f49e2f149d76dd46830321c5b358b4244e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/730
Content-Type: application/json
Authorization: Bearer 805547de5cc5eeabcd34b609dd390c1d9d8196a3c5f5025ab1b54f5228be7fa6
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
    "id": 730,
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
    "created_at": "2016-09-01T13:39:02.443Z",
    "updated_at": "2016-09-01T13:39:02.443Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/730" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 805547de5cc5eeabcd34b609dd390c1d9d8196a3c5f5025ab1b54f5228be7fa6"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/1
Content-Type: application/json
Authorization: Bearer adb5f3191533e2cfd3c5d007c5af6f91ddd46d19c7f64447ce7e0e61e44aea1b
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adb5f3191533e2cfd3c5d007c5af6f91ddd46d19c7f64447ce7e0e61e44aea1b"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/3
Content-Type: application/json
Authorization: Bearer 833b3e1071f8a694ed4b831f4d921a750ece4771340e94acf663b1b550f155d1
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
	-H "Authorization: Bearer 833b3e1071f8a694ed4b831f4d921a750ece4771340e94acf663b1b550f155d1"
```
