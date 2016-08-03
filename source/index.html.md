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
Authorization: Basic Zjg2MjI3NDEzNWUyN2NmYjg2YjBlMmFhMDgxNmY5YTg4NWIyZWVjZmRjN2Iz
N2Q0NTg5NzIzNmQyOGFjYzQ1MzpkMjFhNTFlNTkyYThmMmMyOGJiY2YwMTg5
OTczMzE4YWMwYzUyMGI3MDUxMTdiOWEzMTk0MDkxNjMyYzM4NmQ5

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
	-u f862274135e27cfb86b0e2aa0816f9a885b2eecfdc7b37d45897236d28acc453:d21a51e592a8f2c28bbcf0189973318ac0c520b705117b9a3194091632c386d9
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic Yzc1MGUyMTU3ZTcyYzYyYzA3M2Y0OGU3N2VlYzZlZjI0OGFmNDlhZTc1Yjk3
NGQ3MmRkNTcxNmNhZjJiNjFkYjo4YjYwOTJjYjQ4YzlmYjZjYTcxYzYxYTkw
Y2RmNDAxMDJjOWJlZmExNDE5NGJmZTgxYjE2ODcxYzFkZWVkNWMw

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
	-u c750e2157e72c62c073f48e77eec6ef248af49ae75b974d72dd5716caf2b61db:8b6092cb48c9fb6ca71c61a90cdf40102c9befa14194bfe81b16871c1deed5c0
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"17a75670b4605a478119c97aa807e9d34908c4c729e9cfb443ea1985a709c938","client_secret":"bccbaebe793e005ce9391b6377780c5e1032125d0006b7df48ab692a13d07240"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"17a75670b4605a478119c97aa807e9d34908c4c729e9cfb443ea1985a709c938","client_secret":"bccbaebe793e005ce9391b6377780c5e1032125d0006b7df48ab692a13d07240"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e0626b0c329a24968b20067e3401c6c7cda0f57e960986f4bdcf18ba02678b4f","client_secret":"f94de1ad52452e224929339efdd19bd0e2f9a436b936e7f28d344342b0bbd933"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e0626b0c329a24968b20067e3401c6c7cda0f57e960986f4bdcf18ba02678b4f","client_secret":"f94de1ad52452e224929339efdd19bd0e2f9a436b936e7f28d344342b0bbd933"}' -X POST \
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
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZGU3MTdkOTIzMTQ4MDk1NjdiZGRmNTU0MzU2NGQyYWE2MGJkYWQ0MTljZTdm
MmZlNGQ2NzA1Y2MwZGJkM2ZlMDo0MzVkNzJiMTllNDliNGY3NzM5ZTQ0NmQ0
NjQyNTUyOTA2NmU2MjE5ZjUxOTM0MjdmNTM5OThjNzZjMGZkNWEw

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
  "access_token": "e010d2006863001e93e2b82ab375d1e93297f2ed80f5633deba57cbf691e400b",
  "token_type": "bearer",
  "created_at": 1470244063
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u de717d92314809567bddf5543564d2aa60bdad419ce7f2fe4d6705cc0dbd3fe0:435d72b19e49b4f7739e446d46425529066e6219f5193427f53998c76c0fd5a0
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"001a67ed8c757d0aa87104d201fb598bbe8237239cd709d14f4d7a5622ca8dfe","client_secret":"bc013125dd348cb91cf554b50588af396a569041350606c989577dbd4984dcb6"}
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
  "access_token": "7d3c37d6f85b47597a6a5c1a9db598de78e7a9163d6e41f41508bc9d1e7cdbc7",
  "token_type": "bearer",
  "created_at": 1470244063
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"001a67ed8c757d0aa87104d201fb598bbe8237239cd709d14f4d7a5622ca8dfe","client_secret":"bc013125dd348cb91cf554b50588af396a569041350606c989577dbd4984dcb6"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"7dc0735775a8709f08fa6c532b4b11b61d35565ed6b4416da2427ecf06c99440","client_secret":"e06f61a2e4a85823bea657f413bee64a2d02ee25330a0a46e60430b210fffad4"}
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
  "access_token": "83abc2a885b9f02c537c786b8a76ff2368a228f1e32882417ebdff5b4ad782a2",
  "token_type": "bearer",
  "created_at": 1470244064
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"7dc0735775a8709f08fa6c532b4b11b61d35565ed6b4416da2427ecf06c99440","client_secret":"e06f61a2e4a85823bea657f413bee64a2d02ee25330a0a46e60430b210fffad4"}' -X POST \
	-H "Content-Type: application/json"
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
Authorization: Bearer 2c6cfbf525d454cc43ce6146cda0538f88c6b63a0009ba13c71bf7bb2625f683
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
    "company_id": 30,
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
	-H "Authorization: Bearer 2c6cfbf525d454cc43ce6146cda0538f88c6b63a0009ba13c71bf7bb2625f683"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/12/flashcards
Content-Type: application/json
Authorization: Bearer c2b5dc9c57a6e246a66ee27736eca94365e1df4c97f7e0cd645b31f38e851a89
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":12,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 174,
    "chapter_id": 12,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:54.916Z",
    "created_at": "2016-08-03T17:07:54.916Z",
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
curl "api.goskive.com/v2/chapters/12/flashcards" -d '{"flashcard":{"chapter_id":12,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2b5dc9c57a6e246a66ee27736eca94365e1df4c97f7e0cd645b31f38e851a89"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/13/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 616e6c9beb09ecdd0b36aae496dad72d84aa8ac03636c8761b1c4db6a2bd6988
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

13
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 177,
    "chapter_id": 13,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:55.397Z",
    "created_at": "2016-08-03T17:07:55.397Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/a28055dc6d0fda3323c474444b39e923bd198c25.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/99351b688965ad9f99b4bab8d1e10c2e00a20e69.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/a28055dc6d0fda3323c474444b39e923bd198c25.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/99351b688965ad9f99b4bab8d1e10c2e00a20e69.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/13/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

13
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
	-H "Authorization: Bearer 616e6c9beb09ecdd0b36aae496dad72d84aa8ac03636c8761b1c4db6a2bd6988"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/10/flashcards
Content-Type: application/json
Authorization: Bearer 494ff5c2ce175cdda4871c88b1b2d0488d17a28ea8e76910508438cf631c8dff
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
      "id": 1,
      "obfuscated_id": "vnOJWgI0jGc",
      "author_id": 166,
      "chapter_id": 10,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:54.214Z",
      "created_at": "2016-08-03T17:07:54.214Z",
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
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 166,
      "chapter_id": 10,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:54.235Z",
      "created_at": "2016-08-03T17:07:54.235Z",
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
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 166,
      "chapter_id": 10,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:54.254Z",
      "created_at": "2016-08-03T17:07:54.254Z",
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
curl "api.goskive.com/v2/chapters/10/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 494ff5c2ce175cdda4871c88b1b2d0488d17a28ea8e76910508438cf631c8dff"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer f927de6d57a4751f209d6a35c127b0af9f30c72787059d09ac8db2e133934739
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 134,
    "chapter_id": 5,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:51.576Z",
    "created_at": "2016-08-03T17:07:51.576Z",
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
        "id": 10,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 11,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 12,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 13,
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
curl "api.goskive.com/v2/chapters/5/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f927de6d57a4751f209d6a35c127b0af9f30c72787059d09ac8db2e133934739"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer f7c650652c18b9aecc99960cb53bc08e8679d13a810b8efec8c7de394b344c6a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 3,
    "obfuscated_id": "bco7bNtr_d4",
    "author_id": 128,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:51.115Z",
    "created_at": "2016-08-03T17:07:51.115Z",
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
        "id": 5,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 6,
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
curl "api.goskive.com/v2/chapters/3/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7c650652c18b9aecc99960cb53bc08e8679d13a810b8efec8c7de394b344c6a"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 63d098cc51d6d9aded7e605aa933c6bacc16a123211a42eea21f11f4f6ecf651
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":4,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 131,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:51.349Z",
    "created_at": "2016-08-03T17:07:51.349Z",
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
        "id": 7,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 8,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 9,
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
curl "api.goskive.com/v2/chapters/4/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":4,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63d098cc51d6d9aded7e605aa933c6bacc16a123211a42eea21f11f4f6ecf651"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/6/questions
Content-Type: application/json
Authorization: Bearer 1520f7e291ab4b3eba558a4cf77da8b7addd52bc8190993743dccedfcdcf1d2b
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
      "id": 6,
      "obfuscated_id": "eyxYPTvoIb8",
      "author_id": 137,
      "chapter_id": 6,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:51.830Z",
      "created_at": "2016-08-03T17:07:51.806Z",
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
          "id": 14,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 15,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 138,
      "chapter_id": 6,
      "position": 4,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:51.895Z",
      "created_at": "2016-08-03T17:07:51.871Z",
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
          "id": 16,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 17,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 8,
      "obfuscated_id": "X2B_8FVuFe8",
      "author_id": 139,
      "chapter_id": 6,
      "position": 5,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-08-03T17:07:51.960Z",
      "created_at": "2016-08-03T17:07:51.936Z",
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
          "id": 18,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 19,
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
curl "api.goskive.com/v2/chapters/6/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1520f7e291ab4b3eba558a4cf77da8b7addd52bc8190993743dccedfcdcf1d2b"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/119
Content-Type: application/json
Authorization: Bearer a84bc40129995275c60ca265fa6ac0763c1196ab65b80d38f07e50622d741a53
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
curl "api.goskive.com/v2/chapters/119" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a84bc40129995275c60ca265fa6ac0763c1196ab65b80d38f07e50622d741a53"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/120
Content-Type: application/json
Authorization: Bearer 0c7e99d3416250f7d8894554e56ccaf1d73fb59741a974cc65509b01de2fff49
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
curl "api.goskive.com/v2/chapters/120" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c7e99d3416250f7d8894554e56ccaf1d73fb59741a974cc65509b01de2fff49"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/116
Content-Type: application/json
Authorization: Bearer a38742a7d3ae5834735699ecf0c34900f32d41e8372f16b6f6de11b35a1a7587
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
curl "api.goskive.com/v2/chapters/116" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a38742a7d3ae5834735699ecf0c34900f32d41e8372f16b6f6de11b35a1a7587"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/121
Content-Type: application/json
Authorization: Bearer 09c4bd11d50ea6ecb064ccdbfec71ad69277db59cbdd06f9d56e37bd1441ce84
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/121" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09c4bd11d50ea6ecb064ccdbfec71ad69277db59cbdd06f9d56e37bd1441ce84"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/113
Content-Type: application/json
Authorization: Bearer 4ff0df715cf107a58c092f334eaf7c4090e016b0308bbefecd5ed039ed6d1e9f
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
    "id": 113,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-08-03T17:08:27.451Z",
    "course_id": 199,
    "author_id": 569,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 573,
        "chapter_id": 113,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-08-03T17:08:27.446Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 571,
        "chapter_id": 113,
        "position": 41,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-08-03T17:08:27.330Z",
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
            "id": 90,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 91,
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
curl "api.goskive.com/v2/chapters/113" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ff0df715cf107a58c092f334eaf7c4090e016b0308bbefecd5ed039ed6d1e9f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/117
Content-Type: application/json
Authorization: Bearer c6ea44c3805435812e957fe703efcde3f1fb2c9b13b7f86491937a7b0f6ee08b
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
    "id": 117,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-08-03T17:08:28.390Z",
    "course_id": 203,
    "author_id": 589,
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
curl "api.goskive.com/v2/chapters/117" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6ea44c3805435812e957fe703efcde3f1fb2c9b13b7f86491937a7b0f6ee08b"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 2ac0506be7b9037744ac2664e23486b5ff10d77b9dbeec9f1977959a5c76378a
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
    "id": 3,
    "author_id": 10,
    "reply_to_id": 2,
    "created_at": "2016-08-03T17:07:42.488Z",
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
curl "api.goskive.com/v2/comments/2/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ac0506be7b9037744ac2664e23486b5ff10d77b9dbeec9f1977959a5c76378a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 8c5468a6965e7838f4da78975b8fc8e4c6aba302afdb35f35dda082f21943a87
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
curl "api.goskive.com/v2/comments/1/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c5468a6965e7838f4da78975b8fc8e4c6aba302afdb35f35dda082f21943a87"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer e88e0ffa82040794db2c760dbd2c8edce6ef5cfabb4f7ac4c583a908cdf3b82b
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
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e88e0ffa82040794db2c760dbd2c8edce6ef5cfabb4f7ac4c583a908cdf3b82b"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer c4de578074e53adb3e07623da354351578862a63eadb562f6ef68c07c2716d7f
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
curl "api.goskive.com/v2/comments/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4de578074e53adb3e07623da354351578862a63eadb562f6ef68c07c2716d7f"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 919e130a6c667577214bf0f1a02046da0da496975284c9df581dbff9023565e0
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 919e130a6c667577214bf0f1a02046da0da496975284c9df581dbff9023565e0"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/9/report
Content-Type: application/json
Authorization: Bearer 5fb0ceaf30b353e256886e3e5cbdb997284757ac3aeb755b6826f610f94747dc
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fb0ceaf30b353e256886e3e5cbdb997284757ac3aeb755b6826f610f94747dc"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/11
Content-Type: application/json
Authorization: Bearer ebc7f10e7c50e6a29f4ba0aa484050dc83c3dac0bac85f7e5ad9dd2f92d2b23f
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
    "updated_at": "2016-08-03T17:08:11.195Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebc7f10e7c50e6a29f4ba0aa484050dc83c3dac0bac85f7e5ad9dd2f92d2b23f"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer eb756899d072034c9267b0cf130bb9c205e0474c22f314caeacd9357a9fd8ba0
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
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-08-03T17:08:11.283Z"
    },
    {
      "id": 13,
      "name": "Fake Company Name 12",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-08-03T17:08:11.289Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-08-03T17:08:11.293Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb756899d072034c9267b0cf130bb9c205e0474c22f314caeacd9357a9fd8ba0"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/28/company_profiles
Content-Type: application/json
Authorization: Bearer 7688e810a3edf08b18e2a3898538d80f67ba6a917c6a9227b02835a7612d463f
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
curl "api.goskive.com/v2/companies/28/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7688e810a3edf08b18e2a3898538d80f67ba6a917c6a9227b02835a7612d463f"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer 4dea4dd1a9c095abc770cdd380a6f37c87aa3673d6ade10c278660538f894cf6
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
curl "api.goskive.com/v2/companies/27/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4dea4dd1a9c095abc770cdd380a6f37c87aa3673d6ade10c278660538f894cf6"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer e3046198615e87cc944fb670d2f57989acb8ba348b9eccf518b2e858a4f1eafa
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
      "id": 7,
      "title": "Campaign 7",
      "company_id": 21,
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
      "company_id": 24,
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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3046198615e87cc944fb670d2f57989acb8ba348b9eccf518b2e858a4f1eafa"
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
Authorization: Bearer ba80ab5960aaca2d44743ac026ca1c3733bd57035d8a19ffb7d1bde8231df53e
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
	-H "Authorization: Bearer ba80ab5960aaca2d44743ac026ca1c3733bd57035d8a19ffb7d1bde8231df53e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 58463e14e4e285911cd51e151ef45e5ec5b51e75bccfddbd205aa62344a1e21d
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
    "id": 99,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-08-03T17:08:23.805Z",
    "course_id": 184,
    "author_id": 512,
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
	-H "Authorization: Bearer 58463e14e4e285911cd51e151ef45e5ec5b51e75bccfddbd205aa62344a1e21d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0e845db8fd3c287fb67f460611f4e5c4a085c36c40d859abc9af64a708027049
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
      "id": 76,
      "title": "Clever Chapter Title 64",
      "position": 1,
      "updated_at": "2016-08-03T17:08:21.283Z",
      "course_id": 171,
      "author_id": 462,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 77,
      "title": "Clever Chapter Title 65",
      "position": 2,
      "updated_at": "2016-08-03T17:08:21.309Z",
      "course_id": 171,
      "author_id": 463,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 78,
      "title": "Clever Chapter Title 66",
      "position": 3,
      "updated_at": "2016-08-03T17:08:21.449Z",
      "course_id": 171,
      "author_id": 464,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-08-03T17:08:21.439Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e845db8fd3c287fb67f460611f4e5c4a085c36c40d859abc9af64a708027049"
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
      "id": 82,
      "title": "Clever Chapter Title 70",
      "position": 1,
      "updated_at": "2016-08-03T17:08:22.024Z",
      "course_id": 174,
      "author_id": 476,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 83,
      "title": "Clever Chapter Title 71",
      "position": 2,
      "updated_at": "2016-08-03T17:08:22.047Z",
      "course_id": 174,
      "author_id": 477,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 84,
      "title": "Clever Chapter Title 72",
      "position": 3,
      "updated_at": "2016-08-03T17:08:22.177Z",
      "course_id": 174,
      "author_id": 478,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-08-03T17:08:22.168Z",
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
Authorization: Bearer e455b8363e06ae43639f5e0ad871b95700dd6317c64fcc6552040744f91e9d02
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
      "id": 79,
      "title": "Clever Chapter Title 67",
      "position": 1,
      "updated_at": "2016-08-03T17:08:21.765Z",
      "course_id": 173,
      "author_id": 471,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 80,
      "title": "Clever Chapter Title 68",
      "position": 2,
      "updated_at": "2016-08-03T17:08:21.790Z",
      "course_id": 173,
      "author_id": 472,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 81,
      "title": "Clever Chapter Title 69",
      "position": 3,
      "updated_at": "2016-08-03T17:08:21.814Z",
      "course_id": 173,
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
	-H "Authorization: Bearer e455b8363e06ae43639f5e0ad871b95700dd6317c64fcc6552040744f91e9d02"
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
      "id": 85,
      "title": "Clever Chapter Title 73",
      "position": 1,
      "updated_at": "2016-08-03T17:08:22.382Z",
      "course_id": 176,
      "author_id": 483,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 86,
      "title": "Clever Chapter Title 74",
      "position": 2,
      "updated_at": "2016-08-03T17:08:22.405Z",
      "course_id": 176,
      "author_id": 484,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 87,
      "title": "Clever Chapter Title 75",
      "position": 3,
      "updated_at": "2016-08-03T17:08:22.428Z",
      "course_id": 176,
      "author_id": 485,
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
Authorization: Bearer 713e84fdb34aba8b312ee85a222e6f2a06b793768d1807c2a881486b7d938999
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
    "course_id": 282,
    "user_id": 867,
    "updated_at": "2016-08-03T17:08:44.972Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 713e84fdb34aba8b312ee85a222e6f2a06b793768d1807c2a881486b7d938999"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 4b3157dc15d8e577c6cbf1c1dd4a6f4996d89fc0123edef0fcbed7c5d2c5a702
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
      "id": 5,
      "course_id": 286,
      "user_id": 877,
      "updated_at": "2016-08-03T17:08:45.486Z"
    },
    {
      "id": 6,
      "course_id": 286,
      "user_id": 878,
      "updated_at": "2016-08-03T17:08:45.505Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b3157dc15d8e577c6cbf1c1dd4a6f4996d89fc0123edef0fcbed7c5d2c5a702"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer f9dae8c13f4c346f2bf865d317cbbbe75aa28a8e539cac4d9b18bd47c4f4e968
```

`DELETE /v2/course_requests/:course_request_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/course_requests/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9dae8c13f4c346f2bf865d317cbbbe75aa28a8e539cac4d9b18bd47c4f4e968"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fa45c47f692d69859ecd81a54251c97701c9e0177e1eac2ea6c8a27d78eabd94
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
	-H "Authorization: Bearer fa45c47f692d69859ecd81a54251c97701c9e0177e1eac2ea6c8a27d78eabd94"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 24b3331b61f3571b4188bd634a79af2b088a79bc081d65e5fec0bae3254769a4
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
	-H "Authorization: Bearer 24b3331b61f3571b4188bd634a79af2b088a79bc081d65e5fec0bae3254769a4"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 17f486f6cc6880417b064755a250842c4734e2395209718cbf5bba277eda4efd
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
	-H "Authorization: Bearer 17f486f6cc6880417b064755a250842c4734e2395209718cbf5bba277eda4efd"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4a55f5c750f2cd3229403d55062c07ad2fc7458dd2e8d4d3994d781239454605
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
	-H "Authorization: Bearer 4a55f5c750f2cd3229403d55062c07ad2fc7458dd2e8d4d3994d781239454605"
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
    "creator_id": 845,
    "id": 277,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 257,
    "additional_university_ids": [

    ],
    "topic_id": 289,
    "discipline_id": 290,
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
    "chapters_updated_at": "2016-08-03T17:08:43.023Z",
    "updated_at": "2016-08-03T17:08:43.026Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 181,
        "title": "Clever Chapter Title 157",
        "position": 1,
        "updated_at": "2016-08-03T17:08:42.990Z",
        "course_id": 277,
        "author_id": 845,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-08-03T17:08:42.889Z",
        "questions_updated_at": "2016-08-03T17:08:42.518Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 182,
        "title": "Clever Chapter Title 158",
        "position": 2,
        "updated_at": "2016-08-03T17:08:43.023Z",
        "course_id": 277,
        "author_id": 845,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-08-03T17:08:42.930Z",
        "questions_updated_at": "2016-08-03T17:08:42.640Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 101,
        "obfuscated_id": "PprZyBVq_gc",
        "author_id": 845,
        "chapter_id": 181,
        "position": 89,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:42.518Z",
        "created_at": "2016-08-03T17:08:42.492Z",
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
            "id": 205,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 206,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 103,
        "obfuscated_id": "AVhVflMAvL0",
        "author_id": 845,
        "chapter_id": 182,
        "position": 91,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:42.640Z",
        "created_at": "2016-08-03T17:08:42.615Z",
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
            "id": 209,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 210,
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
Authorization: Bearer 3bed62accc52be8aedcc45d47ca332581308c42a56b3068f0f6670bcbdf39928
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
    "creator_id": 856,
    "id": 279,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 259,
    "additional_university_ids": [

    ],
    "topic_id": 291,
    "discipline_id": 292,
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
    "chapters_updated_at": "2016-08-03T17:08:44.364Z",
    "updated_at": "2016-08-03T17:08:44.367Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 185,
        "title": "Clever Chapter Title 161",
        "position": 1,
        "updated_at": "2016-08-03T17:08:44.330Z",
        "course_id": 279,
        "author_id": 856,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-08-03T17:08:44.252Z",
        "questions_updated_at": "2016-08-03T17:08:43.956Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 186,
        "title": "Clever Chapter Title 162",
        "position": 2,
        "updated_at": "2016-08-03T17:08:44.364Z",
        "course_id": 279,
        "author_id": 856,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-08-03T17:08:44.293Z",
        "questions_updated_at": "2016-08-03T17:08:44.075Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 857,
        "chapter_id": 185,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.230Z",
        "created_at": "2016-08-03T17:08:44.230Z",
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
        "author_id": 857,
        "chapter_id": 186,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.271Z",
        "created_at": "2016-08-03T17:08:44.271Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 857,
        "chapter_id": 185,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.252Z",
        "created_at": "2016-08-03T17:08:44.252Z",
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
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 857,
        "chapter_id": 186,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.293Z",
        "created_at": "2016-08-03T17:08:44.293Z",
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
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 857,
        "chapter_id": 185,
        "position": 101,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:43.903Z",
        "created_at": "2016-08-03T17:08:43.879Z",
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
            "id": 229,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 230,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 114,
        "obfuscated_id": "RwCVsRO9fcs",
        "author_id": 857,
        "chapter_id": 185,
        "position": 102,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:43.956Z",
        "created_at": "2016-08-03T17:08:43.933Z",
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
            "id": 231,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 232,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 857,
        "chapter_id": 186,
        "position": 103,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.021Z",
        "created_at": "2016-08-03T17:08:43.997Z",
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
            "id": 233,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 234,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 116,
        "obfuscated_id": "PhHGVKqnHFA",
        "author_id": 857,
        "chapter_id": 186,
        "position": 104,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-08-03T17:08:44.075Z",
        "created_at": "2016-08-03T17:08:44.051Z",
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
            "id": 235,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 236,
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
	-H "Authorization: Bearer 3bed62accc52be8aedcc45d47ca332581308c42a56b3068f0f6670bcbdf39928"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/280/pin
Content-Type: application/json
Authorization: Bearer dc521456cf5ba1ba9be9bdc776af1f5d52d9b4ca43cb4e05ff9755fa6f0f2f5b
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/280/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc521456cf5ba1ba9be9bdc776af1f5d52d9b4ca43cb4e05ff9755fa6f0f2f5b"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/275/pin
Content-Type: application/json
Authorization: Bearer 21cfe5ea1fe7b8e061249ad7d3d265b590f4822ddcf35b06bd93f07e991f3592
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/275/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21cfe5ea1fe7b8e061249ad7d3d265b590f4822ddcf35b06bd93f07e991f3592"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 861e8e3095c49df4dfe79609326a46713b382e00d9a835fffb7a005fb93e5c9b
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
    "creator_id": 812,
    "id": 263,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 243,
    "additional_university_ids": [

    ],
    "topic_id": 275,
    "discipline_id": 276,
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
    "updated_at": "2016-08-03T17:08:40.020Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 861e8e3095c49df4dfe79609326a46713b382e00d9a835fffb7a005fb93e5c9b"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 4bb872d2aa05d5f5847d733771dc75ce32569759b3e85864f4f0bed67c045459
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
    "id": 32,
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
    "created_at": "2016-08-03T17:07:46.614Z",
    "updated_at": "2016-08-03T17:07:46.614Z",
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
	-H "Authorization: Bearer 4bb872d2aa05d5f5847d733771dc75ce32569759b3e85864f4f0bed67c045459"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 14154a9849a16ba269acabe2dd2cde9262226cc4ecec3ee6787c983f5dde6bd8
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[8]}
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
    "id": 28,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      8
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-08-03T17:07:46.320Z",
    "updated_at": "2016-08-03T17:07:46.359Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[8]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14154a9849a16ba269acabe2dd2cde9262226cc4ecec3ee6787c983f5dde6bd8"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9a31802a66cc8eae97f4a7a85fa2ca43ed7308dea2124d164ddad225631be6ec
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
    "id": 30,
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
    "created_at": "2016-08-03T17:07:46.458Z",
    "updated_at": "2016-08-03T17:07:46.458Z",
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
	-H "Authorization: Bearer 9a31802a66cc8eae97f4a7a85fa2ca43ed7308dea2124d164ddad225631be6ec"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 76b5df02e060ec14028ba88bfaf9f40901453b2fa17295044fe92e591df35a13
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[9]}
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
    "id": 29,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      9
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-08-03T17:07:46.403Z",
    "updated_at": "2016-08-03T17:07:46.403Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[9]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76b5df02e060ec14028ba88bfaf9f40901453b2fa17295044fe92e591df35a13"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 54f7e0c6c74d0cb78a14a067d81d05165ea1cdd572a4e78463765e0e298c2571
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

7
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
    "id": 27,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/307061a1032e9748ea9f476d4cf9c8caa47cc739.jpg",
    "university_id": null,
    "fields_of_study": [
      7
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-08-03T17:07:45.824Z",
    "updated_at": "2016-08-03T17:07:46.256Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/3c4ac871583f137228b39ccf2f3220ae75b10998.jpg",
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

7
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 54f7e0c6c74d0cb78a14a067d81d05165ea1cdd572a4e78463765e0e298c2571"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 7030790cd80cc247499e4bddaad44c4b56bfbcaff3f78a5793d822959d5c1079
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
      "id": 5,
      "bookmarkable_id": 29,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 30,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 31,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7030790cd80cc247499e4bddaad44c4b56bfbcaff3f78a5793d822959d5c1079"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b289a5ad0a072b8751c75eb5f5f76dec4da46b90d99f290cce3142c51646d7ed
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
      "id": 2,
      "title": "Campaign 2",
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
    },
    {
      "id": 1,
      "title": "Campaign 1",
      "company_id": 4,
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b289a5ad0a072b8751c75eb5f5f76dec4da46b90d99f290cce3142c51646d7ed"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 657c5084d56fb4cf00589ebe608f10c88f478b43818a92291b6f1043e48dc71b
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
      "creator_id": 903,
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-226",
      "html_url": "https://goskive.com/course/mit-course-226",
      "slug": "mit-course-226",
      "university_id": 277,
      "additional_university_ids": [

      ],
      "topic_id": 304,
      "discipline_id": 305,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 226",
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
      "updated_at": "2016-08-03T17:08:47.129Z",
      "shortname": "mit-course-226"
    },
    {
      "creator_id": 904,
      "id": 293,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-227",
      "html_url": "https://goskive.com/course/mit-course-227",
      "slug": "mit-course-227",
      "university_id": 278,
      "additional_university_ids": [

      ],
      "topic_id": 305,
      "discipline_id": 306,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 227",
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
      "updated_at": "2016-08-03T17:08:47.218Z",
      "shortname": "mit-course-227"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 657c5084d56fb4cf00589ebe608f10c88f478b43818a92291b6f1043e48dc71b"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cf06c370a5b74267edf17c04d3d37acb8093d34eac9e80172f1052fb81363324
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
      "company_id": 1,
      "company": {
        "id": 1,
        "name": "Fake Company Name 1",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
        "brand_color": "#000000",
        "updated_at": "2016-08-03T17:07:45.123Z"
      },
      "created_at": "2016-08-03T17:07:45.129Z",
      "updated_at": "2016-08-03T17:07:45.129Z"
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
      "company_id": 1,
      "company": {
        "id": 1,
        "name": "Fake Company Name 1",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
        "brand_color": "#000000",
        "updated_at": "2016-08-03T17:07:45.123Z"
      },
      "created_at": "2016-08-03T17:07:45.129Z",
      "updated_at": "2016-08-03T17:07:45.129Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf06c370a5b74267edf17c04d3d37acb8093d34eac9e80172f1052fb81363324"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 37a1c4b83ee23042198c2296f0e79de7990deb3e261f796732fbc5c0ea08e544
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
      "created_at": "2016-08-03T17:08:02.489Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 50,
      "updated_at": "2016-08-03T17:08:02.609Z",
      "author_id": "286",
      "thread_subject_id": "97",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 9,
      "created_at": "2016-08-03T17:08:02.595Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 51,
      "updated_at": "2016-08-03T17:08:02.612Z",
      "author_id": "289",
      "thread_subject_id": "98",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-08-03T17:08:02.812Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-08-03T17:08:02.812Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-08-03T17:08:03.076Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-08-03T17:08:03.076Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 12,
      "created_at": "2016-08-03T17:08:03.287Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-08-03T17:08:03.287Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 13,
      "created_at": "2016-08-03T17:08:03.460Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 19,
      "updated_at": "2016-08-03T17:08:03.460Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-08-03T17:08:03.635Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-08-03T17:08:03.635Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-08-03T17:08:03.800Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 21,
      "updated_at": "2016-08-03T17:08:03.800Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37a1c4b83ee23042198c2296f0e79de7990deb3e261f796732fbc5c0ea08e544"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/7
Content-Type: application/json
Authorization: Bearer 1648c393cdbd3cf6438baf1bbfe43999657d37423102f96a3c7a02bbdb66de2e
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-08-03T16:58:02.000Z"}}
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
    "id": 7,
    "created_at": "2016-08-03T17:08:02.308Z",
    "read_at": "2016-08-03T16:58:02.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 49,
    "updated_at": "2016-08-03T17:08:02.369Z",
    "author_id": "282",
    "thread_subject_id": "96",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/7" -d '{"notification":{"read_at":"2016-08-03T16:58:02.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1648c393cdbd3cf6438baf1bbfe43999657d37423102f96a3c7a02bbdb66de2e"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 773b577d567d4b478933fbfae38758c868ba6e3b4ba3ab6c8ae507947da9081d
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
      "id": 6,
      "course_id": 56,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-08-03T17:07:52.763Z",
      "course_published": true,
      "updated_at": "2016-08-03T17:07:52.754Z"
    },
    {
      "id": 7,
      "course_id": 57,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-08-03T17:07:52.914Z",
      "course_published": true,
      "updated_at": "2016-08-03T17:07:52.906Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 773b577d567d4b478933fbfae38758c868ba6e3b4ba3ab6c8ae507947da9081d"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 3fa88676f11f2cf2294cd0ca7c917bc3f1c6d911df60c6f4a9de98debc1cb81f
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
    "course_id": 58,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-08-03T17:07:53.086Z",
    "course_published": true,
    "updated_at": "2016-08-03T17:07:53.078Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fa88676f11f2cf2294cd0ca7c917bc3f1c6d911df60c6f4a9de98debc1cb81f"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/9
Content-Type: application/json
Authorization: Bearer b89088b368fa0ab7bb452814f44a7eb0d3d975347bcec7907c09fe1dd7b136b7
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
    "course_id": 59,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-08-03T17:07:53.255Z",
    "course_published": true,
    "updated_at": "2016-08-03T17:07:53.248Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/9" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b89088b368fa0ab7bb452814f44a7eb0d3d975347bcec7907c09fe1dd7b136b7"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 8e9c669a4ccdd63f5cc4b7e9dc221e4166852045b283732d017bcfca808e951b
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
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 119,
      "user_id": 880
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 120,
      "user_id": 880
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 880
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 880
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e9c669a4ccdd63f5cc4b7e9dc221e4166852045b283732d017bcfca808e951b"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/66
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
    "id": 66,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 66,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 66
      },
      {
        "id": 67,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 66
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/66" -X GET \
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
      "id": 67,
      "name": "Re-engineered leading edge leverage",
      "name_translations": {
        "en": "Re-engineered leading edge leverage"
      }
    },
    {
      "id": 68,
      "name": "Function-based asymmetric strategy",
      "name_translations": {
        "en": "Function-based asymmetric strategy"
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
PATCH /v2/feedbacks/45/close
Content-Type: application/json
Authorization: Bearer 4f1686e35b7a1bb04b8ad808c09a1993fd4cd85aec3ef2a3e73d11d6e59acee2
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
    "id": 45,
    "user_id": 803,
    "feedbackable_id": 67,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-08-03T17:08:39.408Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/45/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f1686e35b7a1bb04b8ad808c09a1993fd4cd85aec3ef2a3e73d11d6e59acee2"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer feaf3fb516fbcabc5a54f15206b35a5c6df5035750ca9eb3817b83606c30ea5d
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
    "id": 21,
    "user_id": 695,
    "feedbackable_id": 62,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-08-03T17:08:34.536Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer feaf3fb516fbcabc5a54f15206b35a5c6df5035750ca9eb3817b83606c30ea5d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/42
Content-Type: application/json
Authorization: Bearer fb7d3e5cdd54049e55334ff781591714b642bbf4749ebcdcc25963c0a3300976
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
    "id": 42,
    "user_id": 786,
    "feedbackable_id": 64,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-08-03T17:08:38.617Z",
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
curl "api.goskive.com/v2/feedbacks/42" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb7d3e5cdd54049e55334ff781591714b642bbf4749ebcdcc25963c0a3300976"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/fix
Content-Type: application/json
Authorization: Bearer 492f45309354361f111997f9398b8c329e2fb419a2cb4eac6ba8c8696a74d2de
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
	-H "Authorization: Bearer 492f45309354361f111997f9398b8c329e2fb419a2cb4eac6ba8c8696a74d2de"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/fix
Content-Type: application/json
Authorization: Bearer 9cc7e47acd50eaae5aabc2f2d6ed7606d6f7df9eb3c9a220df5ee6269e9368f3
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
curl "api.goskive.com/v2/feedbacks/20/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cc7e47acd50eaae5aabc2f2d6ed7606d6f7df9eb3c9a220df5ee6269e9368f3"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/close
Content-Type: application/json
Authorization: Bearer 8dd3bafb04b156d1418d0d623898432c7317c5f47871dc0c7cbb69dfa8aac8af
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
curl "api.goskive.com/v2/feedbacks/46/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8dd3bafb04b156d1418d0d623898432c7317c5f47871dc0c7cbb69dfa8aac8af"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/43
Content-Type: application/json
Authorization: Bearer 4523c6a0a897bff71fd4a00f72b19c82422eb68be54a1c4349d121141df89c29
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
    "id": 43,
    "user_id": 791,
    "feedbackable_id": 65,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-08-03T17:08:38.895Z",
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
curl "api.goskive.com/v2/feedbacks/43" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4523c6a0a897bff71fd4a00f72b19c82422eb68be54a1c4349d121141df89c29"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/53/comments
Content-Type: application/json
Authorization: Bearer 1fb3a4acbcebb218fcdc062f78fd1b233673273e41093560c16cd66d724db5dd
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
    "id": 57,
    "author_id": 557,
    "reply_to_id": null,
    "created_at": "2016-08-03T17:08:26.584Z",
    "status": "published",
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
curl "api.goskive.com/v2/flashcards/53/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fb3a4acbcebb218fcdc062f78fd1b233673273e41093560c16cd66d724db5dd"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/51/comments
Content-Type: application/json
Authorization: Bearer 3aeea479bd4e5bbaf5e7195ace87f27b17c7b4e6143eafa2fc0e1c8817e8b31a
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
    "id": 56,
    "author_id": 551,
    "reply_to_id": null,
    "created_at": "2016-08-03T17:08:26.109Z",
    "status": "published",
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 18,
      "user_id": 551,
      "feedbackable_id": 51,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:08:26.106Z",
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
curl "api.goskive.com/v2/flashcards/51/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aeea479bd4e5bbaf5e7195ace87f27b17c7b4e6143eafa2fc0e1c8817e8b31a"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer 2e70671aa6be8997ea48f68ebab9861ac45d920e167e110f332eeb50b13753d0
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
      "id": 58,
      "author_id": 566,
      "reply_to_id": null,
      "created_at": "2016-08-03T17:08:27.068Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 567,
      "reply_to_id": null,
      "created_at": "2016-08-03T17:08:27.087Z",
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
curl "api.goskive.com/v2/flashcards/55/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e70671aa6be8997ea48f68ebab9861ac45d920e167e110f332eeb50b13753d0"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/52/comments
Content-Type: application/json
Authorization: Bearer 0bc4791ca5a74cdebe7939fbe6d877124434e2902e39403da48d63d6b8202db4
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
curl "api.goskive.com/v2/flashcards/52/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bc4791ca5a74cdebe7939fbe6d877124434e2902e39403da48d63d6b8202db4"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/43/feedbacks
Content-Type: application/json
Authorization: Bearer a370df74371ae4079214c95eb15f644c53f3c6f82c17b5094599bd12a045e20d
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
    "id": 9,
    "user_id": 361,
    "feedbackable_id": 43,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-08-03T17:08:06.423Z",
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
curl "api.goskive.com/v2/flashcards/43/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a370df74371ae4079214c95eb15f644c53f3c6f82c17b5094599bd12a045e20d"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/36/feedbacks
Content-Type: application/json
Authorization: Bearer ab3bf41a2d9283cfa5baf66ca6ca9350c85757822ef9dae5bb12ad693a194278
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
      "id": 3,
      "user_id": 332,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:08:04.864Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 331,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:08:04.850Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab3bf41a2d9283cfa5baf66ca6ca9350c85757822ef9dae5bb12ad693a194278"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/34/votes
Content-Type: application/json
Authorization: Bearer ae7f1c0673276999515c574fa92af71adf6f4e5ca7eba3f691a188f88d1641c6
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
      "votable_id": 34,
      "user_id": 324
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 34,
      "user_id": 323
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 34,
      "user_id": 322
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/34/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae7f1c0673276999515c574fa92af71adf6f4e5ca7eba3f691a188f88d1641c6"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/27/republish
Content-Type: application/json
Authorization: Bearer 440c65c7a59800cf8ed13f3770543144cec9450806af83b5b0a8be26a5a5961a
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
curl "api.goskive.com/v2/flashcards/27/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 440c65c7a59800cf8ed13f3770543144cec9450806af83b5b0a8be26a5a5961a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/10/bookmark
Content-Type: application/json
Authorization: Bearer e6c23578e6037eec0002019351dee009090fede7db8d6af4cd0591fe6460f1b0
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/10/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6c23578e6037eec0002019351dee009090fede7db8d6af4cd0591fe6460f1b0"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/9
Content-Type: application/json
Authorization: Bearer ccfe41d3e8180db9dcad7d87024b00d48a3c008539e968268e0ca186d8bdb43b
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccfe41d3e8180db9dcad7d87024b00d48a3c008539e968268e0ca186d8bdb43b"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/6/downvote
Content-Type: application/json
Authorization: Bearer ee2bcf54a9e408861da221d8e30794c0580634eda6d9f4c7a9c108cf9f370784
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/6/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee2bcf54a9e408861da221d8e30794c0580634eda6d9f4c7a9c108cf9f370784"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/29
Content-Type: application/json
Authorization: Bearer 08d133672df7568c58f4bbb236b4d02f085905e1fe9a63d4330da4e499efd7e7
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
    "id": 29,
    "obfuscated_id": "rvs1sHrnKS4",
    "author_id": 271,
    "chapter_id": 42,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:08:01.597Z",
    "created_at": "2016-08-03T17:08:01.597Z",
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
curl "api.goskive.com/v2/flashcards/29" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08d133672df7568c58f4bbb236b4d02f085905e1fe9a63d4330da4e499efd7e7"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/31/report
Content-Type: application/json
Authorization: Bearer 2850e5b6d15a22ef07c8fefae67d2841ace2c9382f18f617e17541ac59286d75
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/31/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2850e5b6d15a22ef07c8fefae67d2841ace2c9382f18f617e17541ac59286d75"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/28/bookmark
Content-Type: application/json
Authorization: Bearer 94ba20a8e0e5f941d6a463b0964765ca52b85c48529ad05454382d1ad076c4d2
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94ba20a8e0e5f941d6a463b0964765ca52b85c48529ad05454382d1ad076c4d2"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/7
Content-Type: application/json
Authorization: Bearer 63e8a02ea4bdd666d161281c9e51f8bf9f28ff9341ac2185560126241f5c89cd
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
    "id": 7,
    "obfuscated_id": "XFkue8saGAM",
    "author_id": 199,
    "chapter_id": 20,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:57.650Z",
    "created_at": "2016-08-03T17:07:57.332Z",
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
curl "api.goskive.com/v2/flashcards/7" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63e8a02ea4bdd666d161281c9e51f8bf9f28ff9341ac2185560126241f5c89cd"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/8
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 443ad97c8c91b736d996e1466352b20b9d4afc828555dda658603dfab347d6d1
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 202,
    "chapter_id": 21,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:07:58.074Z",
    "created_at": "2016-08-03T17:07:57.794Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/f6d87433b890696660cb37aa82da9e63ffe3cff2.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/e122eccd0f9618ec0b5d6b1bf2a8eefafbd74c70.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/f6d87433b890696660cb37aa82da9e63ffe3cff2.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/e122eccd0f9618ec0b5d6b1bf2a8eefafbd74c70.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/8" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
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
	-H "Authorization: Bearer 443ad97c8c91b736d996e1466352b20b9d4afc828555dda658603dfab347d6d1"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/30/upvote
Content-Type: application/json
Authorization: Bearer 2551418ad6f1e3b4975985775d31b1bf77cb6fc8b43213a683ded03f2c7ebca3
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/30/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2551418ad6f1e3b4975985775d31b1bf77cb6fc8b43213a683ded03f2c7ebca3"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/flashcards/images/cache/presign
Content-Type: application/json
Authorization: Bearer 0dd7a4ef3e97ce37c31797eac720b3b1c4e91745b9127f5826814e260e30f1ac
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
    "key": "cache/07c84f15063865a903c4cae129caba39",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOC0wM1QxODowNzo1OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8wN2M4NGYxNTA2Mzg2NWE5MDNjNGNhZTEyOWNhYmEzOSJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwODAzL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDgwM1QxNzA3NThaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160803/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160803T170758Z",
    "x-amz-signature": "53452d2ef21be238ee2648777f72c943b0533c499fb49be57d6354a30051453b"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/images/cache/presign" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dd7a4ef3e97ce37c31797eac720b3b1c4e91745b9127f5826814e260e30f1ac"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/4/sign_ups
Content-Type: application/json
Authorization: Bearer 2af203fc1be82f8320ae8dd28fce84c30da0be1fde9e8d7c5bb754a182bb5d5b
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
curl "api.goskive.com/v2/me/jobs/4/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2af203fc1be82f8320ae8dd28fce84c30da0be1fde9e8d7c5bb754a182bb5d5b"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/6/sign_ups
Content-Type: application/json
Authorization: Bearer 2de461c7583152847086c906136a19a57270575f0569bec3729f9ccb30fa8db8
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
curl "api.goskive.com/v2/me/jobs/6/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2de461c7583152847086c906136a19a57270575f0569bec3729f9ccb30fa8db8"
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
{"password":{"reset_password_token":"zxMnWVz1xxGfSZbGRzcQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 441,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-08-03T17:08:18.183Z",
  "updated_at": "2016-08-03T17:08:19.020Z",
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
  "audit_id": 4637
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"zxMnWVz1xxGfSZbGRzcQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
{"password":{"reset_password_token":"XysyawURLGzhvFx3evkm","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "created_at": "2016-08-03T17:08:19.782Z",
  "updated_at": "2016-08-03T17:08:19.952Z",
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
  "audit_id": 4640
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"XysyawURLGzhvFx3evkm","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer 538caa42e2ccf0cdccaafd8da035a49cdcecf363769acd765a38b924629facfb
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
    "id": 46,
    "author_id": 182,
    "reply_to_id": null,
    "created_at": "2016-08-03T17:07:56.212Z",
    "status": "published",
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
curl "api.goskive.com/v2/questions/12/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 538caa42e2ccf0cdccaafd8da035a49cdcecf363769acd765a38b924629facfb"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer a25c6ee5523e2964b96df5d96bab4deb0bcc5ef1a9d928b2bb72d256f860b66f
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
    "id": 45,
    "author_id": 179,
    "reply_to_id": null,
    "created_at": "2016-08-03T17:07:55.872Z",
    "status": "published",
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 179,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:07:55.867Z",
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
curl "api.goskive.com/v2/questions/11/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a25c6ee5523e2964b96df5d96bab4deb0bcc5ef1a9d928b2bb72d256f860b66f"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/15/comments
Content-Type: application/json
Authorization: Bearer 29b12e9846a98acb625ae930a07231e0ebbefc2651c601c8d4a48dd6cfa6db8a
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
      "author_id": 194,
      "reply_to_id": null,
      "created_at": "2016-08-03T17:07:56.946Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 195,
      "reply_to_id": null,
      "created_at": "2016-08-03T17:07:56.966Z",
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
	-H "Authorization: Bearer 29b12e9846a98acb625ae930a07231e0ebbefc2651c601c8d4a48dd6cfa6db8a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/13/comments
Content-Type: application/json
Authorization: Bearer 11255fdb34d5447a7b5a6c61cca7087b93a4c6b42de3d272069e6da6c19cd2aa
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
curl "api.goskive.com/v2/questions/13/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11255fdb34d5447a7b5a6c61cca7087b93a4c6b42de3d272069e6da6c19cd2aa"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/35/feedbacks
Content-Type: application/json
Authorization: Bearer ea3c4136d05437584664fc0cbfe1b4eeb3bf54c096ab4e5f4994423f2895daaa
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
    "id": 10,
    "user_id": 515,
    "feedbackable_id": 35,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-08-03T17:08:24.171Z",
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
curl "api.goskive.com/v2/questions/35/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea3c4136d05437584664fc0cbfe1b4eeb3bf54c096ab4e5f4994423f2895daaa"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/40/feedbacks
Content-Type: application/json
Authorization: Bearer 8baa229fd8c1563fd926400575d5eaf0837d4791c2ba3c3ade65c435c49ec240
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
      "id": 15,
      "user_id": 536,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:08:25.391Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 535,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-08-03T17:08:25.379Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/40/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8baa229fd8c1563fd926400575d5eaf0837d4791c2ba3c3ade65c435c49ec240"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/124/votes
Content-Type: application/json
Authorization: Bearer 7acf2e3c3e6f0829fb2ee801a8438de1bd506d092bb64a6c61153ba2eda05d69
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
      "votable_id": 124,
      "user_id": 913
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 124,
      "user_id": 912
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 124,
      "user_id": 911
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/124/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7acf2e3c3e6f0829fb2ee801a8438de1bd506d092bb64a6c61153ba2eda05d69"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/69/republish
Content-Type: application/json
Authorization: Bearer ee6b3e26c46b69129cc3ad5c4d2b46527baabde8c5ccb72fb7be69d514fc2a1d
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
curl "api.goskive.com/v2/questions/69/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee6b3e26c46b69129cc3ad5c4d2b46527baabde8c5ccb72fb7be69d514fc2a1d"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/66/bookmark
Content-Type: application/json
Authorization: Bearer 2dc23b4b508752f2682169289492db233820e77a18ae1cb4176aa68681ef144a
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/66/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dc23b4b508752f2682169289492db233820e77a18ae1cb4176aa68681ef144a"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/71
Content-Type: application/json
Authorization: Bearer b1fa71cd209d3f9a7482336b1bb2f963664031e52453b4d0a8c4b67eddeea706
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/71" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1fa71cd209d3f9a7482336b1bb2f963664031e52453b4d0a8c4b67eddeea706"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/73/downvote
Content-Type: application/json
Authorization: Bearer 091673ac086c8b5cede24ad11adf6a5151b53c0aeb4602f9d1cbde19b4bb5d09
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/73/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 091673ac086c8b5cede24ad11adf6a5151b53c0aeb4602f9d1cbde19b4bb5d09"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/67
Content-Type: application/json
Authorization: Bearer d45c48be7dd1ee74ca605856cce6ae94fd7f4de2310ada6f0eb404efa05befb1
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
    "id": 67,
    "obfuscated_id": "btMCNJVyvlA",
    "author_id": 661,
    "chapter_id": 140,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:08:32.510Z",
    "created_at": "2016-08-03T17:08:32.486Z",
    "tags": [
      {
        "id": 8,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 7,
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
        "id": 137,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 138,
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
curl "api.goskive.com/v2/questions/67" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d45c48be7dd1ee74ca605856cce6ae94fd7f4de2310ada6f0eb404efa05befb1"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/70/report
Content-Type: application/json
Authorization: Bearer 7ece12a49eca13cd69602b01083db062ccd04fadecfe4f1156bb306247e71e9e
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/70/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ece12a49eca13cd69602b01083db062ccd04fadecfe4f1156bb306247e71e9e"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/72/bookmark
Content-Type: application/json
Authorization: Bearer 97820f1c5cc9a988565ec1e1e59c3bc85a77d47348926bd54029cbf43c835916
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/72/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97820f1c5cc9a988565ec1e1e59c3bc85a77d47348926bd54029cbf43c835916"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/49
Content-Type: application/json
Authorization: Bearer fa79c17b10bf5c47f718f21181f3d5a25d39be3e3779ff780887aadfb0f36b42
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":49,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-08-03T17:08:29.198Z","updated_at":"2016-08-03T17:08:29.223Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":122,"author_id":602,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 49,
    "obfuscated_id": "GNsH7ObIVl0",
    "author_id": 602,
    "chapter_id": 122,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-08-03T17:08:29.310Z",
    "created_at": "2016-08-03T17:08:29.198Z",
    "tags": [
      {
        "id": 2,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 1,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>49, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-08-03T17:08:29.198Z\", \"updated_at\"=>\"2016-08-03T17:08:29.223Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>122, \"author_id\"=>602, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 102,
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
curl "api.goskive.com/v2/questions/49" -d '{"question":{"question":{"id":49,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-08-03T17:08:29.198Z","updated_at":"2016-08-03T17:08:29.223Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":122,"author_id":602,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa79c17b10bf5c47f718f21181f3d5a25d39be3e3779ff780887aadfb0f36b42"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/50/upvote
Content-Type: application/json
Authorization: Bearer 107427f41c4cdcb9c8cee3564b26b3c01dafe7f51756c2af08911ed1197e483d
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 107427f41c4cdcb9c8cee3564b26b3c01dafe7f51756c2af08911ed1197e483d"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer ebc1a2315f646c42cfe0ef53bfed3314e68d79e15cec710aed4d075d0ce91202
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
      "creator_id": 412,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 138,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "discipline_id": 166,
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
      "updated_at": "2016-08-03T17:08:11.030Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebc1a2315f646c42cfe0ef53bfed3314e68d79e15cec710aed4d075d0ce91202"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 00605def57df6cb72b819ab330c5ce69c726957243f10cc0216bb33687ae74c8
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
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-118",
      "html_url": "https://goskive.com/university/uni-118",
      "slug": "uni-118",
      "name": "National School of Pizza",
      "short_name": "Uni 118",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dd30e9d1908c1b7737190dd0b13b0118fbfd0e83.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3d2b6fb4bb6a5135a036b9c1841556d977c17e5a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-08-03T17:08:10.737Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-117",
      "html_url": "https://goskive.com/university/uni-117",
      "slug": "uni-117",
      "name": "National School of Pastry",
      "short_name": "Uni 117",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/549584df18bcc6166f3099c479cb15d1320c128e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3cf492ea3fae834aba879881ee82734c5b7fbf38.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-08-03T17:08:10.720Z",
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
	-H "Authorization: Bearer 00605def57df6cb72b819ab330c5ce69c726957243f10cc0216bb33687ae74c8"
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
      "id": 171,
      "name": "Compatible object-oriented initiative",
      "name_translations": {
        "en": "Compatible object-oriented initiative"
      },
      "discipline_id": 172
    },
    {
      "id": 172,
      "name": "Customizable secondary process improvement",
      "name_translations": {
        "en": "Customizable secondary process improvement"
      },
      "discipline_id": 173
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
GET /v2/topics/173
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
    "id": 173,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 174
  }
}
```



```shell
curl "api.goskive.com/v2/topics/173" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 9978e1b42bd2ef235d0bfbb52d35e5e80f1d5c98471405709e9a0b5b4ad65af4
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
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-254",
      "html_url": "https://goskive.com/university/uni-254",
      "slug": "uni-254",
      "name": "University 191",
      "short_name": "Uni 254",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5aa26f7e4f52a3698c45d9eb3b26ed17d370ea61.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3d90cf539c5651617f18a342d537fae964163306.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-08-03T17:08:46.822Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 275,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-255",
      "html_url": "https://goskive.com/university/uni-255",
      "slug": "uni-255",
      "name": "University 192",
      "short_name": "Uni 255",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/32c35839f1c931f1c861a40dba5692c79527d347.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/fe99545b301f70203e4205fc327b8add39f1658e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-08-03T17:08:46.839Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 276,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-256",
      "html_url": "https://goskive.com/university/uni-256",
      "slug": "uni-256",
      "name": "University 193",
      "short_name": "Uni 256",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e187b40d5c88ebf5f4ae2db7d5fd22938b12dfe6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/faa33f9bffd7dfbce3ef586ec9f34124b0f8022b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-08-03T17:08:46.856Z",
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
	-H "Authorization: Bearer 9978e1b42bd2ef235d0bfbb52d35e5e80f1d5c98471405709e9a0b5b4ad65af4"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 46414e2dc908b0c3b01edf4bd82b383aea3106d1fdddf4c86f880c06c7b46c92
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
    "id": 273,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/95ce47863c09564fb1d903d45e32265f58fad291.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b8ba0e50ec9e8506a381b04b02de55954f460524.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-08-03T17:08:46.680Z",
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
	-H "Authorization: Bearer 46414e2dc908b0c3b01edf4bd82b383aea3106d1fdddf4c86f880c06c7b46c92"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c2d51052cdca772a95c541e8f9c98d93311803dc5e31dc90910a62fe6e308df0
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":126,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 366,
    "id": 119,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 119,
    "additional_university_ids": [

    ],
    "topic_id": 126,
    "discipline_id": 127,
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
    "chapters_updated_at": "2016-08-03T17:08:07.042Z",
    "updated_at": "2016-08-03T17:08:07.050Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 63,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-08-03T17:08:07.013Z",
        "course_id": 119,
        "author_id": 366,
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
        "id": 64,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-08-03T17:08:07.028Z",
        "course_id": 119,
        "author_id": 366,
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
        "id": 65,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-08-03T17:08:07.042Z",
        "course_id": 119,
        "author_id": 366,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":126,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2d51052cdca772a95c541e8f9c98d93311803dc5e31dc90910a62fe6e308df0"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 048df9ed9458887420b4d69b6b422f9d3e49b0bd19963be19fdd1c2ecb5d3187
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":127,"published":false}}
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
    "creator_id": 367,
    "id": 120,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 120,
    "additional_university_ids": [

    ],
    "topic_id": 127,
    "discipline_id": 128,
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
    "updated_at": "2016-08-03T17:08:07.223Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":127,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 048df9ed9458887420b4d69b6b422f9d3e49b0bd19963be19fdd1c2ecb5d3187"
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
      "creator_id": 369,
      "id": 123,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 121,
      "additional_university_ids": [

      ],
      "topic_id": 130,
      "discipline_id": 131,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
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
      "updated_at": "2016-08-03T17:08:07.417Z",
      "shortname": "fu-course-110"
    },
    {
      "creator_id": 369,
      "id": 124,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 121,
      "additional_university_ids": [

      ],
      "topic_id": 131,
      "discipline_id": 132,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
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
      "chapters_updated_at": "2016-08-03T17:08:07.596Z",
      "updated_at": "2016-08-03T17:08:07.598Z",
      "shortname": "fu-course-111"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f235300f4ce883fc9b5e620b238cfbb28752c42ce49ab41ad4310635d0f44728
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
      "creator_id": 396,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 154,
      "discipline_id": 155,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
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
      "updated_at": "2016-08-03T17:08:09.735Z",
      "shortname": "fu-course-134"
    },
    {
      "creator_id": 396,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 155,
      "discipline_id": 156,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "chapters_updated_at": "2016-08-03T17:08:09.909Z",
      "updated_at": "2016-08-03T17:08:09.912Z",
      "shortname": "fu-course-135"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f235300f4ce883fc9b5e620b238cfbb28752c42ce49ab41ad4310635d0f44728"
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
      "creator_id": 374,
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-114",
      "html_url": "https://goskive.com/course/fu-course-114",
      "slug": "fu-course-114",
      "university_id": 122,
      "additional_university_ids": [

      ],
      "topic_id": 134,
      "discipline_id": 135,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 114",
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
      "updated_at": "2016-08-03T17:08:07.798Z",
      "shortname": "fu-course-114"
    },
    {
      "creator_id": 374,
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 122,
      "additional_university_ids": [

      ],
      "topic_id": 135,
      "discipline_id": 136,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 115",
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
      "updated_at": "2016-08-03T17:08:07.841Z",
      "shortname": "fu-course-115"
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
Authorization: Bearer 1d5cfd32a8bea37a09edb591c5340e3306054a286da37078aaf1d51ee0d76e59
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
      "creator_id": 402,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 131,
      "additional_university_ids": [

      ],
      "topic_id": 158,
      "discipline_id": 159,
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
      "updated_at": "2016-08-03T17:08:10.156Z",
      "shortname": "fu-course-138"
    },
    {
      "creator_id": 402,
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 131,
      "additional_university_ids": [

      ],
      "topic_id": 159,
      "discipline_id": 160,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
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
      "updated_at": "2016-08-03T17:08:10.199Z",
      "shortname": "fu-course-139"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d5cfd32a8bea37a09edb591c5340e3306054a286da37078aaf1d51ee0d76e59"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer ef98590b60cfcc6ca31231693dcaa25f90d4e71f103dec941230d52e22929357
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
  "id": 178,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-08-03T17:07:55.477Z",
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
	-H "Authorization: Bearer ef98590b60cfcc6ca31231693dcaa25f90d4e71f103dec941230d52e22929357"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/443
Content-Type: application/json
Authorization: Bearer 114d430daaeb0d98b54a0e4b7d8032e884558a6e36999eb0911b208a91a2b17e
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
    "id": 443,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 147,
    "fields_of_study": [
      178,
      179
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-08-03T17:08:20.103Z",
    "updated_at": "2016-08-03T17:08:20.103Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/443" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 114d430daaeb0d98b54a0e4b7d8032e884558a6e36999eb0911b208a91a2b17e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/445
Content-Type: application/json
Authorization: Bearer 126fa1cd9ea30b28e0a7f70ddd33a4a514709cad22f07d714069633f9a1d7a4a
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
    "id": 445,
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
    "created_at": "2016-08-03T17:08:20.203Z",
    "updated_at": "2016-08-03T17:08:20.203Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/445" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 126fa1cd9ea30b28e0a7f70ddd33a4a514709cad22f07d714069633f9a1d7a4a"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/11
Content-Type: application/json
Authorization: Bearer 360b3c90468ac17a23c55c4eba0dc7f5d6a984e77db2114efd19d933e2e2fbbc
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 360b3c90468ac17a23c55c4eba0dc7f5d6a984e77db2114efd19d933e2e2fbbc"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/10
Content-Type: application/json
Authorization: Bearer 1b814c2a678ef1d20a15ef25775369a8ebc2300468d02734a0a8306e50e5bc74
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
    "id": 10,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 26,
    "user_id": 417
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b814c2a678ef1d20a15ef25775369a8ebc2300468d02734a0a8306e50e5bc74"
```
