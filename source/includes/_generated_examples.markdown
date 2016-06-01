# Skive API Documentation

## changes the feedback state to &#39;closed&#39;

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer 2338b8a0f5c1c705a81f13abe51f7581563e53c436a1fa8d847269ac93240442
```

`PATCH /v2/feedbacks/:feedback_id/close`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/21/close"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2338b8a0f5c1c705a81f13abe51f7581563e53c436a1fa8d847269ac93240442"</code>
## changes the feedback state to &#39;fixed&#39;

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer a636cd9a1c41613549bc6da44d4c5c0428028f9291f6f6bd0c1f2a05808985ab
```

`PATCH /v2/feedbacks/:feedback_id/fix`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/24/fix"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a636cd9a1c41613549bc6da44d4c5c0428028f9291f6f6bd0c1f2a05808985ab"</code>
## changes the password

### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`


#### Parameters


```json
{"password":{"reset_password_token":"6wa4BiUfhU8-sjcrBPRn","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 131,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-06-01T15:49:54.903Z",
  "updated_at": "2016-06-01T15:49:57.568Z",
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
  "audit_id": 28517
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"reset_password_token":"6wa4BiUfhU8-sjcrBPRn","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}'&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## changes the password

### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`


#### Parameters


```json
{"password":{"reset_password_token":"6fmgz6GkKEoiAWuEhBJm","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "created_at": "2016-06-01T15:49:54.253Z",
  "updated_at": "2016-06-01T15:49:54.787Z",
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
  "audit_id": 28516
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"reset_password_token":"6fmgz6GkKEoiAWuEhBJm","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}'&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## creates a bookmark

### Request

#### Endpoint

```
POST /v2/questions/35/bookmarks
Content-Type: application/json
Authorization: Bearer 2f851bf33287de27679658c1179ed8617922a4cfd8f5a1d91cf23fb1b59c5298
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
    "bookmarkable_id": 35,
    "bookmarkable_type": "Question"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/35/bookmarks"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2f851bf33287de27679658c1179ed8617922a4cfd8f5a1d91cf23fb1b59c5298"</code>
## creates a bookmark

### Request

#### Endpoint

```
POST /v2/flashcards/24/bookmarks
Content-Type: application/json
Authorization: Bearer f18d3b596aaba1c41b8e58771b0380902ce88ffd67af59dccca8d51f1f0f5679
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
    "id": 4,
    "bookmarkable_id": 24,
    "bookmarkable_type": "Flashcard"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/24/bookmarks"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;f18d3b596aaba1c41b8e58771b0380902ce88ffd67af59dccca8d51f1f0f5679"</code>
## creates a chapter

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer afaa92c016ff3d77152fb92dbab84eb24ed5ff3a27b25e73e9543d5a12b30f2c
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
    "id": 34,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-06-01T15:49:40.617Z",
    "course_id": 27,
    "author_id": 107,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-d&nbsp;'{"chapter":{"title":"Preparing&nbsp;the&nbsp;oven"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;afaa92c016ff3d77152fb92dbab84eb24ed5ff3a27b25e73e9543d5a12b30f2c"</code>
## creates a chapter

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3d834fee025c5d341c8e979a45aaf2bb7b1fca0b26f50b6edb9bd813bb964407
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
    "id": 33,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-06-01T15:49:40.325Z",
    "course_id": 26,
    "author_id": 105,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-d&nbsp;'{"chapter":{"title":"Preparing&nbsp;the&nbsp;oven"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;3d834fee025c5d341c8e979a45aaf2bb7b1fca0b26f50b6edb9bd813bb964407"</code>
## creates a comment

### Request

#### Endpoint

```
POST /v2/questions/87/comments
Content-Type: application/json
Authorization: Bearer 82b9e2f0fe8553cb07f600c2be4f9413583df727a81392553146d355a49240cc
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
    "id": 19,
    "author_id": 582,
    "reply_to_id": null,
    "created_at": "2016-06-01T15:51:10.357Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/87/comments"&nbsp;-d&nbsp;'{"comment":{"message":"Not&nbsp;sure&nbsp;what&nbsp;this&nbsp;question&nbsp;means."}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;82b9e2f0fe8553cb07f600c2be4f9413583df727a81392553146d355a49240cc"</code>
## creates a comment

### Request

#### Endpoint

```
POST /v2/flashcards/69/comments
Content-Type: application/json
Authorization: Bearer 23f5ed16295cb4d8bbdd2d1045f2b8a2b2bb165f940fd3f8474eb22ae403a812
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
    "id": 23,
    "author_id": 599,
    "reply_to_id": null,
    "created_at": "2016-06-01T15:51:12.605Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/69/comments"&nbsp;-d&nbsp;'{"comment":{"message":"This&nbsp;flashcard&nbsp;is&nbsp;particularly&nbsp;helpful!"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;23f5ed16295cb4d8bbdd2d1045f2b8a2b2bb165f940fd3f8474eb22ae403a812"</code>
## creates a comment with feedback

### Request

#### Endpoint

```
POST /v2/flashcards/70/comments
Content-Type: application/json
Authorization: Bearer 702e6bc29d9f6063177f16e55a26b41b6e1b356819853a0e276207a52079d566
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
    "id": 24,
    "author_id": 602,
    "reply_to_id": null,
    "created_at": "2016-06-01T15:51:13.198Z",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 31,
      "user_id": 602,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:51:13.190Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/70/comments"&nbsp;-d&nbsp;'{"comment":{"message":"Hard&nbsp;to&nbsp;see&nbsp;the&nbsp;formulae.","feedback":{"flags":3}}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;702e6bc29d9f6063177f16e55a26b41b6e1b356819853a0e276207a52079d566"</code>
## creates a comment with feedback

### Request

#### Endpoint

```
POST /v2/questions/88/comments
Content-Type: application/json
Authorization: Bearer ccee31954c6bdcf3a8ba6fdb20c7419f295f169e57bc893868d94a87876f5fbe
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
    "id": 20,
    "author_id": 585,
    "reply_to_id": null,
    "created_at": "2016-06-01T15:51:10.944Z",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 30,
      "user_id": 585,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:51:10.939Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/88/comments"&nbsp;-d&nbsp;'{"comment":{"message":"Really&nbsp;bad&nbsp;grammar.","feedback":{"flags":2}}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ccee31954c6bdcf3a8ba6fdb20c7419f295f169e57bc893868d94a87876f5fbe"</code>
## creates a course request

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer a9b9faf14db196da7a9e9234c876e9d531cfac2630aa9b20260015300fb2a4a6
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
    "id": 2,
    "course_id": 193,
    "user_id": 612,
    "updated_at": "2016-06-01T15:51:15.023Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a9b9faf14db196da7a9e9234c876e9d531cfac2630aa9b20260015300fb2a4a6"</code>
## creates a flashcard

### Request

#### Endpoint

```
POST /v2/chapters/3/flashcards
Content-Type: application/json
Authorization: Bearer 14c5c32b88269d50a8497afe4b22c41597730927b84930f9baf5a066e4617261
```

`POST /v2/chapters/:chapter_id/flashcards`


#### Parameters


```json
{"flashcard":{"chapter_id":3,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 9,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:49:21.501Z",
    "created_at": "2016-06-01T15:49:21.501Z",
    "tags": [

    ],
    "published": false,
    "reported": false,
    "language_code": "fr",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/3/flashcards"&nbsp;-d&nbsp;'{"flashcard":{"chapter_id":3,"front_content":"Function&nbsp;of&nbsp;*eggs*&nbsp;in&nbsp;choux&nbsp;pastry","front_content_html":"Function&nbsp;of&nbsp;&#92;u003cstrong&#92;u003eeggs&#92;u003c/strong&#92;u003e&nbsp;in&nbsp;choux&nbsp;pastry","back_content":"Helps&nbsp;things&nbsp;*raise*","back_content_html":"Helps&nbsp;things&nbsp;&#92;u003cstrong&#92;u003eraise&#92;u003c/strong&#92;u003e","language_code":"fr"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;14c5c32b88269d50a8497afe4b22c41597730927b84930f9baf5a066e4617261"</code>
## creates a flashcard with images

### Request

#### Endpoint

```
POST /v2/chapters/4/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b0feca472835ade56c228940af19ef894d78b88cf80419f721fc8d3180fdc0f7
```

`POST /v2/chapters/:chapter_id/flashcards`


#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

4
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
    "author_id": 12,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:49:22.221Z",
    "created_at": "2016-06-01T15:49:22.221Z",
    "tags": [

    ],
    "published": false,
    "reported": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/634defb0d2c132d5b4bc9bff128f2b6aade56f12.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/b02fd8fcd8ac971bc58b95505f1fd2844c06ab74.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/634defb0d2c132d5b4bc9bff128f2b6aade56f12.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/b02fd8fcd8ac971bc58b95505f1fd2844c06ab74.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/4/flashcards"&nbsp;-d&nbsp;'------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[chapter_id]"<br><br>4<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[front_image]";&nbsp;filename="flashcard_front.jpg"<br>Content-Type:&nbsp;image/jpeg<br>Content-Length:&nbsp;15053<br><br>[uploaded&nbsp;data]<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[back_image]";&nbsp;filename="flashcard_back.jpg"<br>Content-Type:&nbsp;image/jpeg<br>Content-Length:&nbsp;16101<br><br>[uploaded&nbsp;data]<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[language_code]"<br><br>fr<br>------------XnJLe9ZIbbGUYtzPQJ16u1--'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;multipart/form-data;&nbsp;boundary=----------XnJLe9ZIbbGUYtzPQJ16u1"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b0feca472835ade56c228940af19ef894d78b88cf80419f721fc8d3180fdc0f7"</code>
## creates a multiple-choice question

### Request

#### Endpoint

```
POST /v2/chapters/122/questions
Content-Type: application/json
Authorization: Bearer 924c7e5b07f8668039441b81e5af3f177218e1fbd3474d091a29a31c5e5a20d5
```

`POST /v2/chapters/:chapter_id/questions`


#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":122,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 81,
    "obfuscated_id": "jHF1owx40fU",
    "author_id": 552,
    "chapter_id": 122,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:51:06.384Z",
    "created_at": "2016-06-01T15:51:06.384Z",
    "tags": [

    ],
    "published": false,
    "reported": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": true,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 163,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 164,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 165,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 166,
        "position": 4,
        "content": "Eggs",
        "content_html": "<p>Eggs</p>",
        "correct": true
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/122/questions"&nbsp;-d&nbsp;'{"question":{"explanation":"the&nbsp;explanation&nbsp;is&nbsp;simple:&nbsp;**eggs**","chapter_id":122,"question":"How&nbsp;do&nbsp;you&nbsp;make&nbsp;**Choux**?","question_html":"How&nbsp;do&nbsp;you&nbsp;make&nbsp;&#92;u003cstrong&#92;u003eChoux&#92;u003c/strong&#92;u003e?","explanation_html":"the&nbsp;explanation&nbsp;is&nbsp;simple:&nbsp;&#92;u003cstrong&#92;u003eeggs&#92;u003c/strong&#92;u003e","answer_options":[{"content":"Tomatoes","content_html":"&#92;u003cp&#92;u003eTomatoes.&#92;u003c/p&#92;u003e","correct":false},{"content":"Flour","content_html":"&#92;u003cp&#92;u003eFlour&#92;u003c/p&#92;u003e","correct":true},{"content":"Mozzarella","content_html":"&#92;u003cp&#92;u003eMozzarella.&#92;u003c/p&#92;u003e","correct":false},{"content":"Eggs","content_html":"&#92;u003cp&#92;u003eEggs&#92;u003c/p&#92;u003e","correct":true}]}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;924c7e5b07f8668039441b81e5af3f177218e1fbd3474d091a29a31c5e5a20d5"</code>
## creates a published course with chapters

### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e93cf4760d07e75e391f5759447e62d8fc5b77d416ef4a7394c7b8a97a6a65ed
```

`POST /v2/universities/:university_slug_or_id/courses`


#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":178,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 540,
    "id": 168,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 153,
    "additional_university_ids": [

    ],
    "topic_id": 178,
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
    "chapters_updated_at": "2016-06-01T15:51:04.460Z",
    "updated_at": "2016-06-01T15:51:04.483Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 117,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-06-01T15:51:04.403Z",
        "course_id": 168,
        "author_id": 540,
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
        "id": 118,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-06-01T15:51:04.436Z",
        "course_id": 168,
        "author_id": 540,
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
        "id": 119,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-06-01T15:51:04.460Z",
        "course_id": 168,
        "author_id": 540,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;201","topic_id":178,"chapters":[{"title":"Etymology&nbsp;of&nbsp;Choux"},{"title":"Pastry&nbsp;Making&nbsp;in&nbsp;Medieval&nbsp;France"},{"title":"Pastry&nbsp;for&nbsp;Neophytes"}]}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e93cf4760d07e75e391f5759447e62d8fc5b77d416ef4a7394c7b8a97a6a65ed"</code>
## creates a published course, ignoring unpermitted properties

### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9f46fe1f8ab4ae9d666f5ca945f364d6533eccd338cc0ff038d94a58296cf966
```

`POST /v2/universities/:university_slug_or_id/courses`


#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":179,"published":false}}
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
    "creator_id": 541,
    "id": 169,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 154,
    "additional_university_ids": [

    ],
    "topic_id": 179,
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
    "updated_at": "2016-06-01T15:51:04.805Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;201","topic_id":179,"published":false}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;9f46fe1f8ab4ae9d666f5ca945f364d6533eccd338cc0ff038d94a58296cf966"</code>
## creates a question

### Request

#### Endpoint

```
POST /v2/chapters/120/questions
Content-Type: application/json
Authorization: Bearer b5ac7b8326e5d28a7cbcef9e563c1098fe25486c81c463c04fdaf063df873cbb
```

`POST /v2/chapters/:chapter_id/questions`


#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":120,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 546,
    "chapter_id": 120,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:51:05.561Z",
    "created_at": "2016-06-01T15:51:05.561Z",
    "tags": [

    ],
    "published": false,
    "reported": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 158,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 159,
        "position": 2,
        "content": "Flour and eggs",
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/120/questions"&nbsp;-d&nbsp;'{"question":{"explanation":"the&nbsp;explanation&nbsp;is&nbsp;simple:&nbsp;**eggs**","chapter_id":120,"question":"How&nbsp;do&nbsp;you&nbsp;make&nbsp;**Choux**?","question_html":"How&nbsp;do&nbsp;you&nbsp;make&nbsp;&#92;u003cstrong&#92;u003eChoux&#92;u003c/strong&#92;u003e?","explanation_html":"the&nbsp;explanation&nbsp;is&nbsp;simple:&nbsp;&#92;u003cstrong&#92;u003eeggs&#92;u003c/strong&#92;u003e","answer_options":[{"content":"Mozzarella&nbsp;and&nbsp;Tomatoes","content_html":"&#92;u003cp&#92;u003eMozzarella&nbsp;and&nbsp;Tomatoes.&#92;u003c/p&#92;u003e","correct":false},{"content":"Flour&nbsp;and&nbsp;eggs","content_html":"&#92;u003cp&#92;u003eFlour&nbsp;and&nbsp;eggs.&#92;u003c/p&#92;u003e","correct":true}]}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b5ac7b8326e5d28a7cbcef9e563c1098fe25486c81c463c04fdaf063df873cbb"</code>
## creates a question that is not multiple-choice

### Request

#### Endpoint

```
POST /v2/chapters/121/questions
Content-Type: application/json
Authorization: Bearer 8c95800d823f833f26df7a7a3537ad786de5f8ddbf4989a9cd463f13111399f1
```

`POST /v2/chapters/:chapter_id/questions`


#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":121,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 80,
    "obfuscated_id": "94gVa2GR5x8",
    "author_id": 549,
    "chapter_id": 121,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:51:05.969Z",
    "created_at": "2016-06-01T15:51:05.969Z",
    "tags": [

    ],
    "published": false,
    "reported": false,
    "language_code": "de",
    "question": "How many Germans does it take to change a light bulb?",
    "question_html": "How many Germans does it take to change a <strong>light bulb</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Think about German humor.",
    "explanation_html": "Think about German <strong>humor</strong>",
    "answer_options": [
      {
        "id": 160,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 161,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 162,
        "position": 3,
        "content": "Two. One that changes it and one that makes this joke work.",
        "content_html": "<p>Two. One that changes it and one that makes this joke work.</p>",
        "correct": false
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/121/questions"&nbsp;-d&nbsp;'{"question":{"explanation":"Think&nbsp;about&nbsp;German&nbsp;humor.","chapter_id":121,"question":"How&nbsp;many&nbsp;Germans&nbsp;does&nbsp;it&nbsp;take&nbsp;to&nbsp;change&nbsp;a&nbsp;light&nbsp;bulb?","question_html":"How&nbsp;many&nbsp;Germans&nbsp;does&nbsp;it&nbsp;take&nbsp;to&nbsp;change&nbsp;a&nbsp;&#92;u003cstrong&#92;u003elight&nbsp;bulb&#92;u003c/strong&#92;u003e?","explanation_html":"Think&nbsp;about&nbsp;German&nbsp;&#92;u003cstrong&#92;u003ehumor&#92;u003c/strong&#92;u003e","answer_options":[{"content":"None.&nbsp;We&nbsp;use&nbsp;energy&nbsp;saving&nbsp;lamps.","content_html":"&#92;u003cp&#92;u003eNone.&nbsp;We&nbsp;use&nbsp;energy&nbsp;saving&nbsp;lamps.&#92;u003c/p&#92;u003e","correct":false},{"content":"One.&nbsp;We&nbsp;have&nbsp;no&nbsp;humor.","content_html":"&#92;u003cp&#92;u003eOne.&nbsp;We&nbsp;have&nbsp;no&nbsp;humor&#92;u003c/p&#92;u003e","correct":true},{"content":"Two.&nbsp;One&nbsp;that&nbsp;changes&nbsp;it&nbsp;and&nbsp;one&nbsp;that&nbsp;makes&nbsp;this&nbsp;joke&nbsp;work.","content_html":"&#92;u003cp&#92;u003eTwo.&nbsp;One&nbsp;that&nbsp;changes&nbsp;it&nbsp;and&nbsp;one&nbsp;that&nbsp;makes&nbsp;this&nbsp;joke&nbsp;work.&#92;u003c/p&#92;u003e","correct":false}]}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8c95800d823f833f26df7a7a3537ad786de5f8ddbf4989a9cd463f13111399f1"</code>
## creates a reply

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 6630b13bb91baa0b0ab8a11c15474da97d9ec1a0ce159144262634cf59cc0dd0
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
    "id": 2,
    "author_id": 46,
    "reply_to_id": 1,
    "created_at": "2016-06-01T15:49:30.967Z",
    "replies": [

    ],
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/1/replies"&nbsp;-d&nbsp;'{"comment":{"message":"Just&nbsp;keeping&nbsp;the&nbsp;thread&nbsp;alive!"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;6630b13bb91baa0b0ab8a11c15474da97d9ec1a0ce159144262634cf59cc0dd0"</code>
## creates a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`


#### Parameters


```json
{"grant_type":"client_credentials","client_id":"84383fe132d833e28631d8945dbf303845f238e782eaadd6397ac203264ebf4d","client_secret":"cdc73c796eb2a0173a9bbba8804edd046d6e6a5390b64492074945c05556a84f"}
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
  "access_token": "99ea17c0f06e140d643644bd1c35c4bc434da99d477c1db316593f68a44f3353",
  "token_type": "bearer",
  "created_at": 1464796165
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"client_credentials","client_id":"84383fe132d833e28631d8945dbf303845f238e782eaadd6397ac203264ebf4d","client_secret":"cdc73c796eb2a0173a9bbba8804edd046d6e6a5390b64492074945c05556a84f"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## creates a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`


#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"36fe2d965ab15aea87db5d03be21f4bd85939c503c67f24e9c1a201800986503","client_secret":"448a48c34aa24e46ceacb11fa2a7bdf485857ab3688bf63bb63940cf8d7b44c7"}
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
  "access_token": "a2fc45f702a1a30e153ff5f1392debe9befd9c0fe8692ffed30bc6a642fc9154",
  "token_type": "bearer",
  "created_at": 1464796165
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"36fe2d965ab15aea87db5d03be21f4bd85939c503c67f24e9c1a201800986503","client_secret":"448a48c34aa24e46ceacb11fa2a7bdf485857ab3688bf63bb63940cf8d7b44c7"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## creates a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDMxOTFmNzA3ZjhhYzdjMmZjMzFlZTA0ODU4NDBhNTQxMTM4MmVkNzY5NTU4
YjhkOTdmYjYxMmRkZDEyOWVjZTpmOGRlOWY1ZGUxODJlNWU5NTJlNmQ4Njk4
NTYzZjUxNjdiZTA1NmRhMWU0OGM1NzVmNzYxNWY4MTY0MTU2MjE3

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
  "access_token": "26cc134b88da976e013fc4aaa7a054713397066a3de27d0e0ee834a11b508d63",
  "token_type": "bearer",
  "created_at": 1464796169
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-u&nbsp;d3191f707f8ac7c2fc31ee0485840a5411382ed769558b8d97fb612ddd129ece:f8de9f5de182e5e952e6d8698563f5167be056da1e48c575f7615f8164156217</code>
## creates a vote

### Request

#### Endpoint

```
POST /v2/questions/70/votes
Content-Type: application/json
Authorization: Bearer f67703af03b1b2e5f4bea9a81e79557a26d30066d71ba504f68f354824def5b2
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
    "votable_id": 70,
    "user_id": 467
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/70/votes"&nbsp;-d&nbsp;'{"vote":{"type":"DownVote"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;f67703af03b1b2e5f4bea9a81e79557a26d30066d71ba504f68f354824def5b2"</code>
## creates a vote

### Request

#### Endpoint

```
POST /v2/flashcards/11/votes
Content-Type: application/json
Authorization: Bearer 2d36640f51619ffb23c111c958b004924e6acbf77fa1820fb55cf4189cdaa2ba
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
    "id": 4,
    "type": "DownVote",
    "votable_type": "Flashcard",
    "votable_id": 11,
    "user_id": 119
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/11/votes"&nbsp;-d&nbsp;'{"vote":{"type":"DownVote"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2d36640f51619ffb23c111c958b004924e6acbf77fa1820fb55cf4189cdaa2ba"</code>
## creates an unpublished course, respecting permitted properties

### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a04a9eda2c87f6f15f6d968f39fef26fa15f4c3b09e483bb74ce925e2dca06c1
```

`POST /v2/universities/:university_slug_or_id/courses`


#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":180,"published":false}}
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
    "creator_id": 542,
    "id": 170,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 155,
    "additional_university_ids": [

    ],
    "topic_id": 180,
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
    "user_generated": false,
    "published": false,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-06-01T15:51:05.016Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;201","topic_id":180,"published":false}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a04a9eda2c87f6f15f6d968f39fef26fa15f4c3b09e483bb74ce925e2dca06c1"</code>
## creates feedback

### Request

#### Endpoint

```
POST /v2/questions/11/feedbacks
Content-Type: application/json
Authorization: Bearer cdde3e59280f3bac118ccaf56d7826de660efbf9d1bd5ade5669eb0ac870453b
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
    "user_id": 140,
    "feedbackable_id": 11,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-06-01T15:50:02.595Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/11/feedbacks"&nbsp;-d&nbsp;'{"feedback":{"message":"No&nbsp;comprendo","flags":0}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;cdde3e59280f3bac118ccaf56d7826de660efbf9d1bd5ade5669eb0ac870453b"</code>
## creates feedback

### Request

#### Endpoint

```
POST /v2/flashcards/23/feedbacks
Content-Type: application/json
Authorization: Bearer 7449ec3d3713f7394381d046c035fd7d389676e7377a6addc66f80bbd8b166a7
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
    "id": 16,
    "user_id": 293,
    "feedbackable_id": 23,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-06-01T15:50:21.702Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/23/feedbacks"&nbsp;-d&nbsp;'{"feedback":{"message":"No&nbsp;comprendo","flags":0}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;7449ec3d3713f7394381d046c035fd7d389676e7377a6addc66f80bbd8b166a7"</code>
## deletes the bookmark

### Request

#### Endpoint

```
DELETE /v2/bookmarks/5
Content-Type: application/json
Authorization: Bearer d02128466ad79822b6e6e4fb45518d9acf7a06d9bde34683c15347e5b458b482
```

`DELETE /v2/bookmarks/:bookmark_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/bookmarks/5"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d02128466ad79822b6e6e4fb45518d9acf7a06d9bde34683c15347e5b458b482"</code>
## deletes the chapter

### Request

#### Endpoint

```
DELETE /v2/chapters/55
Content-Type: application/json
Authorization: Bearer 6f2f21016ed7da47b80994012785dd536b4d3ae40e7839377d73be5cb1cf5863
```

`DELETE /v2/chapters/:chapter_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/55"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;6f2f21016ed7da47b80994012785dd536b4d3ae40e7839377d73be5cb1cf5863"</code>
## deletes the chapter

### Request

#### Endpoint

```
DELETE /v2/chapters/58
Content-Type: application/json
Authorization: Bearer 17dcdb191a67ac90357278dfe35d9dd9926b8940c71073e67cd19e452b9929f6
```

`DELETE /v2/chapters/:chapter_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/58"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;17dcdb191a67ac90357278dfe35d9dd9926b8940c71073e67cd19e452b9929f6"</code>
## deletes the comment

### Request

#### Endpoint

```
DELETE /v2/comments/9
Content-Type: application/json
Authorization: Bearer 5189f4e12f36bf1957042c8de8802ee7b7eb3277aef7a8d3043b8af4b900f0d7
```

`DELETE /v2/comments/:comment_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/9"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5189f4e12f36bf1957042c8de8802ee7b7eb3277aef7a8d3043b8af4b900f0d7"</code>
## deletes the comment

### Request

#### Endpoint

```
DELETE /v2/comments/10
Content-Type: application/json
Authorization: Bearer 9fc99daa958dfdb7552ecb149a55af6fb2076a8a4fad6d111e413849a15cd9c3
```

`DELETE /v2/comments/:comment_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/10"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;9fc99daa958dfdb7552ecb149a55af6fb2076a8a4fad6d111e413849a15cd9c3"</code>
## deletes the course

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ad181e75981cc8f874f7f091b946f47b4e5a935f215d0ed52db9bdb36afe9498
```

`DELETE /v2/courses/:course_slug_or_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ad181e75981cc8f874f7f091b946f47b4e5a935f215d0ed52db9bdb36afe9498"</code>
## deletes the course

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e3457097162d12ef68d95c09585c6a39870465c9cacf2f0ad835cf05688e2758
```

`DELETE /v2/courses/:course_slug_or_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e3457097162d12ef68d95c09585c6a39870465c9cacf2f0ad835cf05688e2758"</code>
## deletes the course request

### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 9d7fa867558b49d604bdfe91ef4d520ac42176ff07584925fe3915c619bd44d2
```

`DELETE /v2/course_requests/:course_request_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/course_requests/1"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;9d7fa867558b49d604bdfe91ef4d520ac42176ff07584925fe3915c619bd44d2"</code>
## deletes the flashcard

### Request

#### Endpoint

```
DELETE /v2/flashcards/59
Content-Type: application/json
Authorization: Bearer 8706d91ffb41b747e104a1a107d58aa7a7877b32cbadabe78a9237fdfd10327b
```

`DELETE /v2/flashcards/:flashcard_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/59"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8706d91ffb41b747e104a1a107d58aa7a7877b32cbadabe78a9237fdfd10327b"</code>
## deletes the question

### Request

#### Endpoint

```
DELETE /v2/questions/1
Content-Type: application/json
Authorization: Bearer adb96ce892a932a736504ec515e8ecba805e5481b344910f96c79cc6fff66faf
```

`DELETE /v2/questions/:question_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/1"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;adb96ce892a932a736504ec515e8ecba805e5481b344910f96c79cc6fff66faf"</code>
## deletes the vote

### Request

#### Endpoint

```
DELETE /v2/votes/5
Content-Type: application/json
Authorization: Bearer d3b12198aa327b7b7840b6d51b648b2c8a463525ba71d877a763d6092c34d676
```

`DELETE /v2/votes/:vote_id`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/votes/5"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d3b12198aa327b7b7840b6d51b648b2c8a463525ba71d877a763d6092c34d676"</code>
## does not change fields of study ids if no value is given

### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 361399e061b0f3de472ae5d02e4cb0684a8dd2d6441830a68e5da14bdb3bd1f1
```

`PATCH /v2/me/user`


#### Parameters


```json
{"email":"magnus@gmail.sk"}
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
    "id": 255,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      74
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-01T15:50:15.961Z",
    "updated_at": "2016-06-01T15:50:16.098Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-d&nbsp;'{"email":"magnus@gmail.sk"}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;361399e061b0f3de472ae5d02e4cb0684a8dd2d6441830a68e5da14bdb3bd1f1"</code>
## does not change the feedback state

### Request

#### Endpoint

```
PATCH /v2/feedbacks/29/fix
Content-Type: application/json
Authorization: Bearer b66e4e613293d6a11cb77f8593aa31570555cbf31479392d565e80a9c6378d55
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/29/fix"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b66e4e613293d6a11cb77f8593aa31570555cbf31479392d565e80a9c6378d55"</code>
## does not change the feedback state

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer 232a7b1b70bab5c1a6f4ccb189b2e35874850aaf898bfa8d0051194d173df734
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/23/close"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;232a7b1b70bab5c1a6f4ccb189b2e35874850aaf898bfa8d0051194d173df734"</code>
## does not change the password

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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"password":"new-passw0rd","password_confirmation":"new-passw0rd","reset_password_token":"invalidt0ken"}}'&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not create a chapter

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e887df07c624252f319fc7ab114afe819f3ea1e478c9fce532d1a0cea3b43eb7
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-d&nbsp;'{"chapter":{"title":"Preparing&nbsp;the&nbsp;oven"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e887df07c624252f319fc7ab114afe819f3ea1e478c9fce532d1a0cea3b43eb7"</code>
## does not create a comment with a missing message

### Request

#### Endpoint

```
POST /v2/flashcards/71/comments
Content-Type: application/json
Authorization: Bearer 7ffd94cc7b20a911a5cd53d76ccbf21904ea8ffb60132ee9e779ceaf0198f0d8
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/71/comments"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;7ffd94cc7b20a911a5cd53d76ccbf21904ea8ffb60132ee9e779ceaf0198f0d8"</code>
## does not create a comment with a missing message

### Request

#### Endpoint

```
POST /v2/questions/89/comments
Content-Type: application/json
Authorization: Bearer b917323521b45d46eb80b288d742dbafe100923487acdc76b9de7aca25467fda
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/89/comments"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b917323521b45d46eb80b288d742dbafe100923487acdc76b9de7aca25467fda"</code>
## does not create a reply with a missing message

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 0232435fbae98f5cb6d69d1ec9f4e5afa62a4a26434b28190f476e340226a4d7
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/3/replies"&nbsp;-d&nbsp;'{}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;0232435fbae98f5cb6d69d1ec9f4e5afa62a4a26434b28190f476e340226a4d7"</code>
## does not create a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`


#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"75a459bd87989460bd349d085f6daecd976e83fe38598aab212b5199a3a04cb0","client_secret":"4b34fccf41cb67d2ceb8ff78ecada6c0639b428c2168fa6589b6f95e91c227e4"}
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"75a459bd87989460bd349d085f6daecd976e83fe38598aab212b5199a3a04cb0","client_secret":"4b34fccf41cb67d2ceb8ff78ecada6c0639b428c2168fa6589b6f95e91c227e4"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not create a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`


#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a828322cd83fb718f022c95ed9369ed30456ced1a148bb6e380b0dc9d5039d4d","client_secret":"ff836f645f7e5514ff01a554d5120ab606fba3eadaffd6290d08c4d282115034"}
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a828322cd83fb718f022c95ed9369ed30456ced1a148bb6e380b0dc9d5039d4d","client_secret":"ff836f645f7e5514ff01a554d5120ab606fba3eadaffd6290d08c4d282115034"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not create a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YWE3MzIxNWI5N2ZiMDJmZTlkNDJlYzdiNDJjYmE3NTIxMWY4YzI0NzU0ODUy
ZmYxOThmODVmMjg2NjAyN2M3NTphOThlYjBjYjU2Yjg1MTQ2YWQ0NGFmODU3
MmY1ODExMzAyYzg0MjExM2VjYjgwMzJmOTI0ZGE0OWYxNzIxYmFk

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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-u&nbsp;aa73215b97fb02fe9d42ec7b42cba75211f8c24754852ff198f85f2866027c75:a98eb0cb56b85146ad44af8572f5811302c842113ecb8032f924da49f1721bad</code>
## does not create a token

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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not create a token

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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not create a token

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OGMwNGFiMWZiMjhlNWEwNTFjYTE5MTE2OWI2NGM0N2FkOTFiYmI3NjVlZTUx
MTk5ZTAyMmU2OWQzMTU4ZjIyYjo2ZmU1NTY0MTNiNmJiZjFkYTg3MzQyOGE2
YmM2NjkyNmRkNzg3MDhjY2YyMTczMjE1MjRlMWQwMzU3NmMxNWFm

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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/oauth/token"&nbsp;-d&nbsp;'{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-u&nbsp;8c04ab1fb28e5a051ca191169b64c47ad91bbb765ee51199e022e69d3158f22b:6fe556413b6bbf1da873428a6bc66926dd78708ccf217321524e1d03576c15af</code>
## does not delete the chapter

### Request

#### Endpoint

```
DELETE /v2/chapters/57
Content-Type: application/json
Authorization: Bearer 35c447e52cf4b0659d38b5ffd05a6c75bd581e84fda7d658ff9689edbd249000
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/57"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;35c447e52cf4b0659d38b5ffd05a6c75bd581e84fda7d658ff9689edbd249000"</code>
## does not delete the chapter

### Request

#### Endpoint

```
DELETE /v2/chapters/56
Content-Type: application/json
Authorization: Bearer 3ae49cec8cfe018452d1885475b89589257432fbf84ecb7a4d31d4e44a81e393
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/56"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;3ae49cec8cfe018452d1885475b89589257432fbf84ecb7a4d31d4e44a81e393"</code>
## does not delete the comment

### Request

#### Endpoint

```
DELETE /v2/comments/11
Content-Type: application/json
Authorization: Bearer e176265a12526172c8c4d84898e9f4530cfd7264b334392884899ebd6fe7c1a0
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/11"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e176265a12526172c8c4d84898e9f4530cfd7264b334392884899ebd6fe7c1a0"</code>
## does not delete the course

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 922f8ee59bdb051515ffbf16d4a23f00dab261823821e01b714701c0f78159ed
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;922f8ee59bdb051515ffbf16d4a23f00dab261823821e01b714701c0f78159ed"</code>
## does not delete the course

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 78a1fe535f4f6db5b4617b47673fc0dd3bda51e12a03457fe7c0b1b9293fe78c
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;DELETE&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;78a1fe535f4f6db5b4617b47673fc0dd3bda51e12a03457fe7c0b1b9293fe78c"</code>
## does not pin the course (create a user course)

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4f429e52d43da6539a6b2a5231e9bce13c4866a4173714203506b2e2053c204e
```

`POST /v2/me/user_courses`


#### Parameters


```json
{"user_course":{"course_id":179,"pinned":true}}
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses"&nbsp;-d&nbsp;'{"user_course":{"course_id":179,"pinned":true}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4f429e52d43da6539a6b2a5231e9bce13c4866a4173714203506b2e2053c204e"</code>
## does not publish feedbackable

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 10f8d1c62abacba0762ed1a4a6069647755819baad9758b3606894abc8c1aa6e
```

`PATCH /v2/feedbacks/:feedback_id/fix`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/27/fix"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;10f8d1c62abacba0762ed1a4a6069647755819baad9758b3606894abc8c1aa6e"</code>
## does not publish feedbackable

### Request

#### Endpoint

```
PATCH /v2/feedbacks/18/close
Content-Type: application/json
Authorization: Bearer 27e0cda4937aaf65941efbaf4e85a37a9f8a688d556bf4d557538fcd7700b53e
```

`PATCH /v2/feedbacks/:feedback_id/close`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/18/close"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;27e0cda4937aaf65941efbaf4e85a37a9f8a688d556bf4d557538fcd7700b53e"</code>
## does not republish the comment

### Request

#### Endpoint

```
PUT /v2/comments/7/republish
Content-Type: application/json
Authorization: Bearer 1cdfab82bdf9c734944c1602bab1ee567423d9c278689c5d8082a151fe88dafc
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/7/republish"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1cdfab82bdf9c734944c1602bab1ee567423d9c278689c5d8082a151fe88dafc"</code>
## does not send a password reset email

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





### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"email":"jan.turnosky@hotmail.com"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## does not sign up the user

### Request

#### Endpoint

```
POST /v2/me/widgets/1/sign_ups
Content-Type: application/json
Authorization: Bearer cced5df1de8066a7aafc0ca0703a4e2a429510c06a3ec9d540ab390621ecfe3a
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/widgets/1/sign_ups"&nbsp;-d&nbsp;'{"sign_up":{"email_address":""}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;cced5df1de8066a7aafc0ca0703a4e2a429510c06a3ec9d540ab390621ecfe3a"</code>
## does not sign up the user

### Request

#### Endpoint

```
POST /v2/me/jobs/6/sign_ups
Content-Type: application/json
Authorization: Bearer 5512b93c10bd5468d76a7fbf18528402699e752c24204860511c39e2a0c8339d
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/jobs/6/sign_ups"&nbsp;-d&nbsp;'{"sign_up":{"email_address":""}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5512b93c10bd5468d76a7fbf18528402699e752c24204860511c39e2a0c8339d"</code>
## does not unpublish flashcard

### Request

#### Endpoint

```
POST /v2/flashcards/22/feedbacks
Content-Type: application/json
Authorization: Bearer 23a5754c61a88ce4a786bda88a5f39bb20d8efc4465ac864730a9e2773db6094
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
    "id": 15,
    "user_id": 290,
    "feedbackable_id": 22,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-06-01T15:50:20.771Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/22/feedbacks"&nbsp;-d&nbsp;'{"feedback":{"message":"No&nbsp;comprendo","flags":0}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;23a5754c61a88ce4a786bda88a5f39bb20d8efc4465ac864730a9e2773db6094"</code>
## does not unpublish question

### Request

#### Endpoint

```
POST /v2/questions/10/feedbacks
Content-Type: application/json
Authorization: Bearer 8ec4de47a8ae5d659e2c127a12a453ec63c3a3d55768b6b280161618eaa1e233
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
    "id": 1,
    "user_id": 137,
    "feedbackable_id": 10,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-06-01T15:50:01.705Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/10/feedbacks"&nbsp;-d&nbsp;'{"feedback":{"message":"No&nbsp;comprendo","flags":0}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8ec4de47a8ae5d659e2c127a12a453ec63c3a3d55768b6b280161618eaa1e233"</code>
## does not update the chapter

### Request

#### Endpoint

```
PATCH /v2/chapters/52
Content-Type: application/json
Authorization: Bearer 3c00c66cd91068fa6d2bc5ec84b1a10ce9a5144d814b4732065451f2eba9f8e0
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/52"&nbsp;-d&nbsp;'{"chapter":{"title":"Eggs&nbsp;and&nbsp;Flour"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;3c00c66cd91068fa6d2bc5ec84b1a10ce9a5144d814b4732065451f2eba9f8e0"</code>
## does not update the course

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ed3d01cb4d4c88d8985fb117b77503a8eede1331e96b80889d55ee1e43bb76af
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;102","language_code":"fr"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ed3d01cb4d4c88d8985fb117b77503a8eede1331e96b80889d55ee1e43bb76af"</code>
## pins the course (create a user course)

### Request

#### Endpoint

```
POST /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9b775b8835f9bee6f9892269a420e20d6b8d5a93ed83131ddc91684a73bb70ea
```

`POST /v2/me/user_courses`


#### Parameters


```json
{"user_course":{"course_id":180,"pinned":true}}
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
    "id": 8,
    "course_id": 180,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-06-01T15:51:08.544Z",
    "course_published": true,
    "updated_at": "2016-06-01T15:51:08.531Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses"&nbsp;-d&nbsp;'{"user_course":{"course_id":180,"pinned":true}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;9b775b8835f9bee6f9892269a420e20d6b8d5a93ed83131ddc91684a73bb70ea"</code>
## provides a collection including counts, permissions

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e020c5f66ac43abb1c9d50ce35f6b451ce95fa4c862fd97a080f5cf3eb182440
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
      "creator_id": 503,
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-87",
      "html_url": "https://goskive.com/course/fu-course-87",
      "slug": "fu-course-87",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "topic_id": 146,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 87",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-06-01T15:50:57.951Z",
      "shortname": "fu-course-87"
    },
    {
      "creator_id": 503,
      "id": 137,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-88",
      "html_url": "https://goskive.com/course/fu-course-88",
      "slug": "fu-course-88",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "topic_id": 147,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 88",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-06-01T15:50:58.016Z",
      "shortname": "fu-course-88"
    },
    {
      "creator_id": 504,
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-89",
      "html_url": "https://goskive.com/course/fu-course-89",
      "slug": "fu-course-89",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "topic_id": 148,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
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
      "updated_at": "2016-06-01T15:50:58.125Z",
      "shortname": "fu-course-89"
    },
    {
      "creator_id": 504,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-90",
      "html_url": "https://goskive.com/course/fu-course-90",
      "slug": "fu-course-90",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "topic_id": 149,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 90",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
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
      "chapters_updated_at": "2016-06-01T15:50:58.446Z",
      "updated_at": "2016-06-01T15:50:58.449Z",
      "shortname": "fu-course-90"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e020c5f66ac43abb1c9d50ce35f6b451ce95fa4c862fd97a080f5cf3eb182440"</code>
## provides a collection including counts, permissions

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 900377c5f4948c66566bd4e9d642ce8bb0e36be7d6c26c8fab54f42d0dbe6e34
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
      "id": 26,
      "title": "Clever Chapter Title 22",
      "position": 1,
      "updated_at": "2016-06-01T15:49:38.792Z",
      "course_id": 22,
      "author_id": 89,
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
      "id": 27,
      "title": "Clever Chapter Title 23",
      "position": 2,
      "updated_at": "2016-06-01T15:49:38.833Z",
      "course_id": 22,
      "author_id": 90,
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
      "id": 28,
      "title": "Clever Chapter Title 24",
      "position": 3,
      "updated_at": "2016-06-01T15:49:39.061Z",
      "course_id": 22,
      "author_id": 91,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-06-01T15:49:38.934Z",
      "questions_updated_at": "2016-06-01T15:49:39.049Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;900377c5f4948c66566bd4e9d642ce8bb0e36be7d6c26c8fab54f42d0dbe6e34"</code>
## provides a collection including counts, permissions

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ae3bde859408a08edf3017ba663e61b24eba01b3cea1b662550b89021a382c64
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
      "creator_id": 521,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 147,
      "additional_university_ids": [

      ],
      "topic_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
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
      "updated_at": "2016-06-01T15:51:00.861Z",
      "shortname": "fu-course-105"
    },
    {
      "creator_id": 521,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 147,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
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
      "chapters_updated_at": "2016-06-01T15:51:01.232Z",
      "updated_at": "2016-06-01T15:51:01.237Z",
      "shortname": "fu-course-106"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ae3bde859408a08edf3017ba663e61b24eba01b3cea1b662550b89021a382c64"</code>
## provides a collection including counts, permissions

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
      "creator_id": 514,
      "id": 146,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-97",
      "html_url": "https://goskive.com/course/fu-course-97",
      "slug": "fu-course-97",
      "university_id": 144,
      "additional_university_ids": [

      ],
      "topic_id": 156,
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
      "updated_at": "2016-06-01T15:50:59.491Z",
      "shortname": "fu-course-97"
    },
    {
      "creator_id": 514,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 144,
      "additional_university_ids": [

      ],
      "topic_id": 157,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
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
      "chapters_updated_at": "2016-06-01T15:50:59.806Z",
      "updated_at": "2016-06-01T15:50:59.810Z",
      "shortname": "fu-course-98"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides a collection including counts, permissions

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
      "id": 14,
      "title": "Clever Chapter Title 10",
      "position": 1,
      "updated_at": "2016-06-01T15:49:35.763Z",
      "course_id": 16,
      "author_id": 64,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 15,
      "title": "Clever Chapter Title 11",
      "position": 2,
      "updated_at": "2016-06-01T15:49:35.809Z",
      "course_id": 16,
      "author_id": 65,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 16,
      "title": "Clever Chapter Title 12",
      "position": 3,
      "updated_at": "2016-06-01T15:49:36.094Z",
      "course_id": 16,
      "author_id": 66,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-06-01T15:49:36.068Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides a collection including counts, permissions

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2f5041b567406708739d2778faef0b4194930dc619ccf20c42484ea03ee1de06
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
      "creator_id": 531,
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-113",
      "html_url": "https://goskive.com/course/fu-course-113",
      "slug": "fu-course-113",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 172,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 113",
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
      "updated_at": "2016-06-01T15:51:02.591Z",
      "shortname": "fu-course-113"
    },
    {
      "creator_id": 531,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-114",
      "html_url": "https://goskive.com/course/fu-course-114",
      "slug": "fu-course-114",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 173,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 114",
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
      "chapters_updated_at": "2016-06-01T15:51:03.063Z",
      "updated_at": "2016-06-01T15:51:03.072Z",
      "shortname": "fu-course-114"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2f5041b567406708739d2778faef0b4194930dc619ccf20c42484ea03ee1de06"</code>
## provides a collection including counts, permissions

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d50dfc331505e4246c152ab3ed39ed4d249771d30228b3c7f4c02b452e27ebeb
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
      "id": 20,
      "title": "Clever Chapter Title 16",
      "position": 1,
      "updated_at": "2016-06-01T15:49:37.309Z",
      "course_id": 19,
      "author_id": 75,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 21,
      "title": "Clever Chapter Title 17",
      "position": 2,
      "updated_at": "2016-06-01T15:49:37.402Z",
      "course_id": 19,
      "author_id": 76,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 22,
      "title": "Clever Chapter Title 18",
      "position": 3,
      "updated_at": "2016-06-01T15:49:37.843Z",
      "course_id": 19,
      "author_id": 77,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-06-01T15:49:37.812Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d50dfc331505e4246c152ab3ed39ed4d249771d30228b3c7f4c02b452e27ebeb"</code>
## provides a collection of chapter flashcards

### Request

#### Endpoint

```
GET /v2/chapters/2/flashcards
Content-Type: application/json
Authorization: Bearer 50301458427adc8e6227086cb303b666448f695a8a349357afa185c1a2d8acf7
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
      "author_id": 4,
      "chapter_id": 2,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:49:20.841Z",
      "created_at": "2016-06-01T15:49:20.841Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    },
    {
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 4,
      "chapter_id": 2,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:49:20.869Z",
      "created_at": "2016-06-01T15:49:20.869Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    },
    {
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 4,
      "chapter_id": 2,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:49:20.895Z",
      "created_at": "2016-06-01T15:49:20.895Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
      "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/2/flashcards"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;50301458427adc8e6227086cb303b666448f695a8a349357afa185c1a2d8acf7"</code>
## provides a collection of chapter questions

### Request

#### Endpoint

```
GET /v2/chapters/124/questions
Content-Type: application/json
Authorization: Bearer 3da59b281eac8620acb468a8e6169ebce210427b876f058398797252e279d502
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
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 558,
      "chapter_id": 124,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:51:07.200Z",
      "created_at": "2016-06-01T15:51:07.127Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 167,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 168,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 83,
      "obfuscated_id": "FCSR-nKROLo",
      "author_id": 559,
      "chapter_id": 124,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:51:07.316Z",
      "created_at": "2016-06-01T15:51:07.271Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 169,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 170,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 84,
      "obfuscated_id": "Hu6DTUHzhWo",
      "author_id": 560,
      "chapter_id": 124,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-06-01T15:51:07.456Z",
      "created_at": "2016-06-01T15:51:07.412Z",
      "tags": [

      ],
      "published": true,
      "reported": false,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 171,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 172,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/124/questions"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;3da59b281eac8620acb468a8e6169ebce210427b876f058398797252e279d502"</code>
## provides a collection of companies

### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer e984ce5a1e0adf41a6962185fb37c2e4484e41147de54a03e893de296aa55852
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
      "id": 21,
      "name": "Fake Company Name 17",
      "logo_url": null,
      "brand_color": "#000000",
      "updated_at": "2016-06-01T15:51:14.394Z"
    },
    {
      "id": 22,
      "name": "Fake Company Name 18",
      "logo_url": null,
      "brand_color": "#000000",
      "updated_at": "2016-06-01T15:51:14.413Z"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e984ce5a1e0adf41a6962185fb37c2e4484e41147de54a03e893de296aa55852"</code>
## provides a collection of company profiles

### Request

#### Endpoint

```
GET /v2/companies/8/company_profiles
Content-Type: application/json
Authorization: Bearer 612ca0158199e74e13a3de5341cf649ad099b8353ba9bc0b106cf308a0ee4c42
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
      "id": 6,
      "display_priority": 1,
      "published": false,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/e454a32c998f7d7ac27f091147bbb511cdb6f8e8.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/0d72c01d65a8bf6733c1fdf8c672243b6d546a9e.png",
      "widgets": [

      ]
    },
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 5,
      "display_priority": 1,
      "published": false,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/43cd8331a2a1101475dca8b52baf14565bda8d25.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/36ab23184d8eb9448413fbe09f112b2034c6db2d.png",
      "widgets": [

      ]
    },
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 4,
      "display_priority": 1,
      "published": false,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/b7227ba08020eaf424f385a68712e11390fe76a3.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/15a47e0f0d046fb9c95772f170325321f8fb4d6d.png",
      "widgets": [

      ]
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies/8/company_profiles"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;612ca0158199e74e13a3de5341cf649ad099b8353ba9bc0b106cf308a0ee4c42"</code>
## provides a collection of course campaigns

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 34d211b6b784594a98b6962eb5aa1e6a2554b7268c80717ba4d3d30eaab4473c
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
      "company_id": 17,
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
      "company_id": 20,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;34d211b6b784594a98b6962eb5aa1e6a2554b7268c80717ba4d3d30eaab4473c"</code>
## provides a collection of course chapters

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8fad0ef3436ad65d399a7fa1a6b78ea5a0a02593c4fed2c04bb08982fae76c37
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
      "id": 29,
      "title": "Clever Chapter Title 25",
      "position": 1,
      "updated_at": "2016-06-01T15:49:39.371Z",
      "course_id": 23,
      "author_id": 96,
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
      "id": 30,
      "title": "Clever Chapter Title 26",
      "position": 2,
      "updated_at": "2016-06-01T15:49:39.410Z",
      "course_id": 23,
      "author_id": 97,
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
      "id": 31,
      "title": "Clever Chapter Title 27",
      "position": 3,
      "updated_at": "2016-06-01T15:49:39.449Z",
      "course_id": 23,
      "author_id": 98,
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
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8fad0ef3436ad65d399a7fa1a6b78ea5a0a02593c4fed2c04bb08982fae76c37"</code>
## provides a collection of course chapters

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fc150e81c301f8355ed5d2c46c24b248b878beef48e4444ead3b32bc85dba77e
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
      "id": 23,
      "title": "Clever Chapter Title 19",
      "position": 1,
      "updated_at": "2016-06-01T15:49:38.375Z",
      "course_id": 21,
      "author_id": 84,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 24,
      "title": "Clever Chapter Title 20",
      "position": 2,
      "updated_at": "2016-06-01T15:49:38.434Z",
      "course_id": 21,
      "author_id": 85,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 25,
      "title": "Clever Chapter Title 21",
      "position": 3,
      "updated_at": "2016-06-01T15:49:38.483Z",
      "course_id": 21,
      "author_id": 86,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;fc150e81c301f8355ed5d2c46c24b248b878beef48e4444ead3b32bc85dba77e"</code>
## provides a collection of course chapters

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
      "id": 17,
      "title": "Clever Chapter Title 13",
      "position": 1,
      "updated_at": "2016-06-01T15:49:36.840Z",
      "course_id": 18,
      "author_id": 71,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 18,
      "title": "Clever Chapter Title 14",
      "position": 2,
      "updated_at": "2016-06-01T15:49:36.910Z",
      "course_id": 18,
      "author_id": 72,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 19,
      "title": "Clever Chapter Title 15",
      "position": 3,
      "updated_at": "2016-06-01T15:49:36.977Z",
      "course_id": 18,
      "author_id": 73,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides a collection of course course requests

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c53267f55848f3a8693febc7ccab571da61eb04c61a1293dc6c097000f4b72e7
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
      "id": 4,
      "course_id": 195,
      "user_id": 616,
      "updated_at": "2016-06-01T15:51:15.538Z"
    },
    {
      "id": 5,
      "course_id": 195,
      "user_id": 617,
      "updated_at": "2016-06-01T15:51:15.575Z"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;c53267f55848f3a8693febc7ccab571da61eb04c61a1293dc6c097000f4b72e7"</code>
## provides a collection of current user bookmarks

### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer e74c7d471f382067169498ca52f26e3f8ecb78238662d80a1af6a0baf186beb6
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
      "bookmarkable_id": 21,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 22,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 23,
      "bookmarkable_type": "Question"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/bookmarks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e74c7d471f382067169498ca52f26e3f8ecb78238662d80a1af6a0baf186beb6"</code>
## provides a collection of current user courses

### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer a87f528b2708cefad18a9b5026b2f0f09a937d823ed7974ab4f0b5b3a7c261bf
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
      "creator_id": 39,
      "id": 10,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-6",
      "html_url": "https://goskive.com/course/mit-course-6",
      "slug": "mit-course-6",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "topic_id": 10,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
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
      "updated_at": "2016-06-01T15:49:29.496Z",
      "shortname": "mit-course-6"
    },
    {
      "creator_id": 40,
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-7",
      "html_url": "https://goskive.com/course/mit-course-7",
      "slug": "mit-course-7",
      "university_id": 11,
      "additional_university_ids": [

      ],
      "topic_id": 11,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
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
      "updated_at": "2016-06-01T15:49:29.617Z",
      "shortname": "mit-course-7"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a87f528b2708cefad18a9b5026b2f0f09a937d823ed7974ab4f0b5b3a7c261bf"</code>
## provides a collection of current user jobs

### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer c64237b2eb30dd1f2a0c9b4b99af843c82046ae7047ed959668c898c9fff88c1
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
      "company_id": 3,
      "created_at": "2016-06-01T15:49:43.139Z",
      "updated_at": "2016-06-01T15:49:43.139Z"
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
      "company_id": 3,
      "created_at": "2016-06-01T15:49:43.139Z",
      "updated_at": "2016-06-01T15:49:43.139Z"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/jobs"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;c64237b2eb30dd1f2a0c9b4b99af843c82046ae7047ed959668c898c9fff88c1"</code>
## provides a collection of current user notifications

### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 739946856a150db5f7790eb441a2269f67d2f582e1c39c569f2be6563bd3cb96
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
      "id": 15,
      "created_at": "2016-06-01T15:50:47.241Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 15,
      "updated_at": "2016-06-01T15:50:47.470Z",
      "author_id": "432",
      "thread_subject_id": "112",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-06-01T15:50:47.447Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 16,
      "updated_at": "2016-06-01T15:50:47.486Z",
      "author_id": "435",
      "thread_subject_id": "113",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-06-01T15:50:47.922Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-06-01T15:50:47.922Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-06-01T15:50:48.362Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-06-01T15:50:48.362Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 22,
      "created_at": "2016-06-01T15:50:48.734Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-06-01T15:50:48.734Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 23,
      "created_at": "2016-06-01T15:50:49.055Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 65,
      "updated_at": "2016-06-01T15:50:49.055Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-06-01T15:50:49.365Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 66,
      "updated_at": "2016-06-01T15:50:49.365Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-06-01T15:50:49.655Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 67,
      "updated_at": "2016-06-01T15:50:49.655Z"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/notifications"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;739946856a150db5f7790eb441a2269f67d2f582e1c39c569f2be6563bd3cb96"</code>
## provides a collection of current user user courses

### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8eadc5f9225c227513cb17ed36fd5820baf9e7f8229e98fe64abc4d5816a0006
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
      "id": 9,
      "course_id": 181,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-06-01T15:51:08.775Z",
      "course_published": true,
      "updated_at": "2016-06-01T15:51:08.763Z"
    },
    {
      "id": 10,
      "course_id": 182,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-06-01T15:51:08.922Z",
      "course_published": true,
      "updated_at": "2016-06-01T15:51:08.906Z"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8eadc5f9225c227513cb17ed36fd5820baf9e7f8229e98fe64abc4d5816a0006"</code>
## provides a collection of current user votes

### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 2fbb10e2542604156f7bf2939f7a6d21f6a1bfd6a8d92d4c04b2cd3d4b340811
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
      "votable_id": 71,
      "user_id": 486
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 72,
      "user_id": 486
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 73,
      "user_id": 486
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 74,
      "user_id": 486
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2fbb10e2542604156f7bf2939f7a6d21f6a1bfd6a8d92d4c04b2cd3d4b340811"</code>
## provides a collection of disciplines

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
      "id": 204,
      "name": "Distributed incremental implementation",
      "name_translations": {
        "en": "Distributed incremental implementation"
      }
    },
    {
      "id": 205,
      "name": "Virtual high-level interface",
      "name_translations": {
        "en": "Virtual high-level interface"
      }
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/disciplines"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## provides a collection of flashcard comments

### Request

#### Endpoint

```
GET /v2/flashcards/68/comments
Content-Type: application/json
Authorization: Bearer 366460ec1c79a9841bd6e58d47b95a8db72d1b6d915475996f22001020a40fb4
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
      "id": 21,
      "author_id": 597,
      "reply_to_id": null,
      "created_at": "2016-06-01T15:51:12.107Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 598,
      "reply_to_id": null,
      "created_at": "2016-06-01T15:51:12.176Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/68/comments"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;366460ec1c79a9841bd6e58d47b95a8db72d1b6d915475996f22001020a40fb4"</code>
## provides a collection of flashcard feedbacks

### Request

#### Endpoint

```
GET /v2/flashcards/21/feedbacks
Content-Type: application/json
Authorization: Bearer 93969aede73ac0fd4281d24aeb8d28116ad18b4aacd7d01f7f9c8edf1b0992b0
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
      "id": 14,
      "user_id": 286,
      "feedbackable_id": 21,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:20.089Z",
      "flags": 1
    },
    {
      "id": 13,
      "user_id": 285,
      "feedbackable_id": 21,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:20.054Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/21/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;93969aede73ac0fd4281d24aeb8d28116ad18b4aacd7d01f7f9c8edf1b0992b0"</code>
## provides a collection of flashcard feedbacks

### Request

#### Endpoint

```
GET /v2/flashcards/16/feedbacks
Content-Type: application/json
Authorization: Bearer 6772e7d8fb9de8f30e3b50797eeb47645129caa7a5845540fd41d075e7a85d92
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
      "id": 10,
      "user_id": 264,
      "feedbackable_id": 16,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:17.830Z",
      "flags": 1
    },
    {
      "id": 9,
      "user_id": 263,
      "feedbackable_id": 16,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:17.802Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/16/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;6772e7d8fb9de8f30e3b50797eeb47645129caa7a5845540fd41d075e7a85d92"</code>
## provides a collection of flashcard feedbacks

### Request

#### Endpoint

```
GET /v2/flashcards/18/feedbacks
Content-Type: application/json
Authorization: Bearer 347a951b983fff12711ed5316f86eab35b1ea8589e67d3f9e98c72baf8f7de8d
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
      "id": 12,
      "user_id": 272,
      "feedbackable_id": 18,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:18.573Z",
      "flags": 1
    },
    {
      "id": 11,
      "user_id": 271,
      "feedbackable_id": 18,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:18.554Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/18/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;347a951b983fff12711ed5316f86eab35b1ea8589e67d3f9e98c72baf8f7de8d"</code>
## provides a collection of flashcard votes

### Request

#### Endpoint

```
GET /v2/flashcards/10/votes
Content-Type: application/json
Authorization: Bearer 786187685419726aca58b6ad2226e057ab950c2e6c7ff30d88ee87c4322eb1cd
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 10,
      "user_id": 118
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 10,
      "user_id": 117
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 10,
      "user_id": 116
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/10/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;786187685419726aca58b6ad2226e057ab950c2e6c7ff30d88ee87c4322eb1cd"</code>
## provides a collection of question comments

### Request

#### Endpoint

```
GET /v2/questions/85/comments
Content-Type: application/json
Authorization: Bearer b11d3923c351e0eccd83ff6c9bfc6bfc891f4b8bf630d4544b5794615c88af4b
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
      "id": 17,
      "author_id": 577,
      "reply_to_id": null,
      "created_at": "2016-06-01T15:51:09.450Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 578,
      "reply_to_id": null,
      "created_at": "2016-06-01T15:51:09.528Z",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/85/comments"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b11d3923c351e0eccd83ff6c9bfc6bfc891f4b8bf630d4544b5794615c88af4b"</code>
## provides a collection of question feedbacks

### Request

#### Endpoint

```
GET /v2/questions/13/feedbacks
Content-Type: application/json
Authorization: Bearer 25596be050fbe342da842f1ad21c883908161ba9cebc8df59a893279cb85c39e
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
      "id": 4,
      "user_id": 153,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:03.925Z",
      "flags": 1
    },
    {
      "id": 3,
      "user_id": 152,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:03.902Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/13/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;25596be050fbe342da842f1ad21c883908161ba9cebc8df59a893279cb85c39e"</code>
## provides a collection of question feedbacks

### Request

#### Endpoint

```
GET /v2/questions/17/feedbacks
Content-Type: application/json
Authorization: Bearer 5a5a0974d1d462cd92f2a8fa9f33cac73bc36ca4f9cc867369600da13f32a38f
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
      "user_id": 172,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:05.726Z",
      "flags": 1
    },
    {
      "id": 7,
      "user_id": 171,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:05.704Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/17/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5a5a0974d1d462cd92f2a8fa9f33cac73bc36ca4f9cc867369600da13f32a38f"</code>
## provides a collection of question feedbacks

### Request

#### Endpoint

```
GET /v2/questions/15/feedbacks
Content-Type: application/json
Authorization: Bearer 1b47a31eaee846b6a4f02f1af3c2291e99e16242ff2f3da2085794e964d64f9c
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
      "user_id": 164,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:04.905Z",
      "flags": 1
    },
    {
      "id": 5,
      "user_id": 163,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-06-01T15:50:04.891Z",
      "flags": 1
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/15/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1b47a31eaee846b6a4f02f1af3c2291e99e16242ff2f3da2085794e964d64f9c"</code>
## provides a collection of question votes

### Request

#### Endpoint

```
GET /v2/questions/68/votes
Content-Type: application/json
Authorization: Bearer 4ab10dfb7f4f007d786a26702a08f03bf5442bef3ef98fcba199dc0f92637459
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
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 68,
      "user_id": 463
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 68,
      "user_id": 462
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 68,
      "user_id": 461
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/68/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4ab10dfb7f4f007d786a26702a08f03bf5442bef3ef98fcba199dc0f92637459"</code>
## provides a collection of topics

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
      "id": 31,
      "name": "Visionary demand-driven internet solution",
      "name_translations": {
        "en": "Visionary demand-driven internet solution"
      },
      "discipline_id": 31
    },
    {
      "id": 32,
      "name": "Progressive next generation synergy",
      "name_translations": {
        "en": "Progressive next generation synergy"
      },
      "discipline_id": 32
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/topics"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## provides a collection of universities

### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 169914283df3ba06bcede1fa06aaac59a7a5220a6a3d2f18da9960ca372e4286
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
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-38",
      "html_url": "https://goskive.com/university/uni-38",
      "slug": "uni-38",
      "name": "University 19",
      "short_name": "Uni 38",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/787c71b072d0ce40e1e2bb9802f2149b627b3e66.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/f463301a186d609139a3c7768efe3fd07dafa7cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-01T15:50:00.208Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 36,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-36",
      "html_url": "https://goskive.com/university/uni-36",
      "slug": "uni-36",
      "name": "University 17",
      "short_name": "Uni 36",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/8719b75788b2276bfd5917a821b96227f3736f76.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/8d84e9c640e414068b212b7f65b7535ba2e50631.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-01T15:50:00.142Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-37",
      "html_url": "https://goskive.com/university/uni-37",
      "slug": "uni-37",
      "name": "University 18",
      "short_name": "Uni 37",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/5a31c14aaa327411e5112f2ad95027a91d5042c7.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/2e7c4ffa5b19a1a35726a8406ceb24468f8f7904.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-01T15:50:00.176Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;169914283df3ba06bcede1fa06aaac59a7a5220a6a3d2f18da9960ca372e4286"</code>
## provides a collection of university courses

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 828cee491a33ee62698eed886be3e715a486fa1486f20840507e9d2643a9e5f1
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
      "creator_id": 528,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
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
      "updated_at": "2016-06-01T15:51:01.889Z",
      "shortname": "fu-course-109"
    },
    {
      "creator_id": 528,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 169,
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
      "updated_at": "2016-06-01T15:51:01.970Z",
      "shortname": "fu-course-110"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;828cee491a33ee62698eed886be3e715a486fa1486f20840507e9d2643a9e5f1"</code>
## provides a collection of university courses

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
      "creator_id": 519,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-101",
      "html_url": "https://goskive.com/course/fu-course-101",
      "slug": "fu-course-101",
      "university_id": 145,
      "additional_university_ids": [

      ],
      "topic_id": 160,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 101",
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
      "updated_at": "2016-06-01T15:51:00.253Z",
      "shortname": "fu-course-101"
    },
    {
      "creator_id": 519,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 145,
      "additional_university_ids": [

      ],
      "topic_id": 161,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
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
      "updated_at": "2016-06-01T15:51:00.376Z",
      "shortname": "fu-course-102"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides a collection of university courses

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 83ccbcf5c8876ed26209c6faff079332a16840b112e24cd4e2fba0d72ca81166
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
      "creator_id": 510,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-91",
      "html_url": "https://goskive.com/course/fu-course-91",
      "slug": "fu-course-91",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "topic_id": 150,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 91",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-06-01T15:50:58.888Z",
      "shortname": "fu-course-91"
    },
    {
      "creator_id": 510,
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-92",
      "html_url": "https://goskive.com/course/fu-course-92",
      "slug": "fu-course-92",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "topic_id": 151,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 92",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-06-01T15:50:58.954Z",
      "shortname": "fu-course-92"
    },
    {
      "creator_id": 511,
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-93",
      "html_url": "https://goskive.com/course/fu-course-93",
      "slug": "fu-course-93",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "topic_id": 152,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 93",
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
      "updated_at": "2016-06-01T15:50:59.041Z",
      "shortname": "fu-course-93"
    },
    {
      "creator_id": 511,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-94",
      "html_url": "https://goskive.com/course/fu-course-94",
      "slug": "fu-course-94",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "topic_id": 153,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 94",
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
      "updated_at": "2016-06-01T15:50:59.106Z",
      "shortname": "fu-course-94"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;83ccbcf5c8876ed26209c6faff079332a16840b112e24cd4e2fba0d72ca81166"</code>
## provides a collection of university courses

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1aa19371e463a66758c029e2218e4efc7925c1de542dca5eeda89392bf3f57ca
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
      "creator_id": 538,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-117",
      "html_url": "https://goskive.com/course/fu-course-117",
      "slug": "fu-course-117",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 117",
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
      "updated_at": "2016-06-01T15:51:03.850Z",
      "shortname": "fu-course-117"
    },
    {
      "creator_id": 538,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-118",
      "html_url": "https://goskive.com/course/fu-course-118",
      "slug": "fu-course-118",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 118",
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
      "updated_at": "2016-06-01T15:51:03.930Z",
      "shortname": "fu-course-118"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1aa19371e463a66758c029e2218e4efc7925c1de542dca5eeda89392bf3f57ca"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/flashcards/67/comments
Content-Type: application/json
Authorization: Bearer cedfaddbcc770c7756ea3546a350220d17b39ef4490b3452138ec0275b26e903
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/67/comments"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;cedfaddbcc770c7756ea3546a350220d17b39ef4490b3452138ec0275b26e903"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b23a4f73058f65974844ea635f68b7597f01625bc119c9048d9075a78b0a148d
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b23a4f73058f65974844ea635f68b7597f01625bc119c9048d9075a78b0a148d"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ceff972e551d629dae247f3a6e7457586cebc55b2a9fd0f8fd7c405326318752
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ceff972e551d629dae247f3a6e7457586cebc55b2a9fd0f8fd7c405326318752"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1da2aaeb98f2fe020e1b03e6dfccbe666637df7ecd0aa3f80f87ca2b38a30df6
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1da2aaeb98f2fe020e1b03e6dfccbe666637df7ecd0aa3f80f87ca2b38a30df6"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/flashcards/20/feedbacks
Content-Type: application/json
Authorization: Bearer bb987fe91826fdec72bb6054d24bd2380809ff4dda863e3a4c3d6d3b31bbd004
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/20/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;bb987fe91826fdec72bb6054d24bd2380809ff4dda863e3a4c3d6d3b31bbd004"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/flashcards/19/feedbacks
Content-Type: application/json
Authorization: Bearer 2db122b2e5070814d0e8366abb4a11b9c782c8a53d58cfb2a846b36afe673a0c
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/19/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2db122b2e5070814d0e8366abb4a11b9c782c8a53d58cfb2a846b36afe673a0c"</code>
## provides an empty collection

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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/chapters"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f85bdce05cd4ea9df73039239a5cd1b198f586706d6405f987a0e10040ebb909
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;f85bdce05cd4ea9df73039239a5cd1b198f586706d6405f987a0e10040ebb909"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/flashcards/17/feedbacks
Content-Type: application/json
Authorization: Bearer 02ea296c264e783aa5e767622a41d83084284a3271d08a84a9cb2b4875bd4b39
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/17/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;02ea296c264e783aa5e767622a41d83084284a3271d08a84a9cb2b4875bd4b39"</code>
## provides an empty collection

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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/topics"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/flashcards/9/votes
Content-Type: application/json
Authorization: Bearer 59b952d9b230c948361a62c0a981c14ec522f659122b59faafb560b470d43a5e
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/9/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;59b952d9b230c948361a62c0a981c14ec522f659122b59faafb560b470d43a5e"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 46054fa5c410129f185e003953e9f21c14df7c07bf68e926c667c2095f163ae9
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;46054fa5c410129f185e003953e9f21c14df7c07bf68e926c667c2095f163ae9"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a6dc1b2ec1e5dfaa6f7671633afd3dac9ec7fb64a8330f802b0439e68be678e3
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/jobs"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a6dc1b2ec1e5dfaa6f7671633afd3dac9ec7fb64a8330f802b0439e68be678e3"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 35ee0d1c42971ded979028d4e527ada36ea74ec1b248ec5621db773ad9fe49eb
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;35ee0d1c42971ded979028d4e527ada36ea74ec1b248ec5621db773ad9fe49eb"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/chapters/123/questions
Content-Type: application/json
Authorization: Bearer d0235f3f61133d6b833147040d7bceb146900b7a7c5c510be0b071d67d0cb090
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/123/questions"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d0235f3f61133d6b833147040d7bceb146900b7a7c5c510be0b071d67d0cb090"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f798e6a5dcbf452fcc8527f7c232867c7c2c206cb58843e0e22c9a1c7f1c0397
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;f798e6a5dcbf452fcc8527f7c232867c7c2c206cb58843e0e22c9a1c7f1c0397"</code>
## provides an empty collection

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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer e23aec59175e31821c89a683213cf0d77601a26313130d74ba766d786b9daab3
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e23aec59175e31821c89a683213cf0d77601a26313130d74ba766d786b9daab3"</code>
## provides an empty collection

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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/disciplines"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer d926c17e4cb879012d276c3a4c0dc01f072d6526eaf841bf3e45027ad7ca196c
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d926c17e4cb879012d276c3a4c0dc01f072d6526eaf841bf3e45027ad7ca196c"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2bd03864d0e0b017e2c34b823851afa843c7a5446213f67c8fd1782c6064f747
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/bookmarks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2bd03864d0e0b017e2c34b823851afa843c7a5446213f67c8fd1782c6064f747"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/questions/12/feedbacks
Content-Type: application/json
Authorization: Bearer c46479fc545763514e80b55655f39b9d2b75658a2f5bdc4f618ffd0def7abaae
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/12/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;c46479fc545763514e80b55655f39b9d2b75658a2f5bdc4f618ffd0def7abaae"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/questions/14/feedbacks
Content-Type: application/json
Authorization: Bearer c53961252995a06b6bdc82a83901f6f72740280ea6af615a34df6546cd68c3f8
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/14/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;c53961252995a06b6bdc82a83901f6f72740280ea6af615a34df6546cd68c3f8"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer baeaeb34872cc5fafc75637994c1d688b50bcdbd04a8b9fce262fc764ccba92a
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;baeaeb34872cc5fafc75637994c1d688b50bcdbd04a8b9fce262fc764ccba92a"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a2d98bfbed39113dabf7e87dd6c4d49ee684b7c09955f93b51de4ad31973b38c
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin/courses"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a2d98bfbed39113dabf7e87dd6c4d49ee684b7c09955f93b51de4ad31973b38c"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/questions/86/comments
Content-Type: application/json
Authorization: Bearer 36acd8b72b8e373374bb16363441501c7d14036a0ed093666fb9703c95af6771
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/86/comments"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;36acd8b72b8e373374bb16363441501c7d14036a0ed093666fb9703c95af6771"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer f367fe0ff6bb74174a1e8e4ad50fb7a4d292b2c47e9ac3d925dc7db031081b7b
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/notifications"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;f367fe0ff6bb74174a1e8e4ad50fb7a4d292b2c47e9ac3d925dc7db031081b7b"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/search/universities?query=un
Content-Type: application/json
Authorization: Bearer d4f020884f47010f7ef88a60a97f28bb0aad0c6f769d80d92bdd0134cd85cb6c
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/search/universities?query=un"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d4f020884f47010f7ef88a60a97f28bb0aad0c6f769d80d92bdd0134cd85cb6c"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/questions/16/feedbacks
Content-Type: application/json
Authorization: Bearer ecf6c247afa7d02dcec200a54df82628343584e67322dd27812d01657dd94810
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/16/feedbacks"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ecf6c247afa7d02dcec200a54df82628343584e67322dd27812d01657dd94810"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/questions/69/votes
Content-Type: application/json
Authorization: Bearer 1c89ee0b7fa0e44f7293b74e79d2fc1f63e0e780fbd61d6a138e5e7f7ada59c7
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/69/votes"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1c89ee0b7fa0e44f7293b74e79d2fc1f63e0e780fbd61d6a138e5e7f7ada59c7"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/search/courses?query=un
Content-Type: application/json
Authorization: Bearer 4c0b4f2be07d37681961ff1d300d2937f497b4c7b9d79d1ef90ef79be6191c62
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/search/courses?query=un"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4c0b4f2be07d37681961ff1d300d2937f497b4c7b9d79d1ef90ef79be6191c62"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/companies/7/company_profiles
Content-Type: application/json
Authorization: Bearer 48a7a75ba5d44e66f00167eda2ac1fc48e7f6dafc4b71fab55dcd649efaad5c4
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies/7/company_profiles"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;48a7a75ba5d44e66f00167eda2ac1fc48e7f6dafc4b71fab55dcd649efaad5c4"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/chapters/1/flashcards
Content-Type: application/json
Authorization: Bearer ebfe250637739c9081ebe88c0f089944b08e95121da58a77acac704412ff8f8c
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/1/flashcards"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ebfe250637739c9081ebe88c0f089944b08e95121da58a77acac704412ff8f8c"</code>
## provides an empty collection

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer ab6516458431952c37da6e377b19b12381846caf9e25d4c3c1b766aba98ed9ba
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

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;ab6516458431952c37da6e377b19b12381846caf9e25d4c3c1b766aba98ed9ba"</code>
## provides company profiles with embedded widgets

### Request

#### Endpoint

```
GET /v2/companies/6/company_profiles
Content-Type: application/json
Authorization: Bearer 8001d339a9f22aec9b0a970e41923322a7067efef86160fab4dcd6f6e59524be
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
      "published": false,
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
          "company_id": 6,
          "created_at": "2016-06-01T15:50:07.145Z",
          "updated_at": "2016-06-01T15:50:07.145Z",
          "type": "job_posting"
        }
      ]
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies/6/company_profiles"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8001d339a9f22aec9b0a970e41923322a7067efef86160fab4dcd6f6e59524be"</code>
## publishes feedbackable

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer cb9962973abe8842d27a4eb0c92e800cfa32b29ea6fcc0b9b7cf995969e0aad9
```

`PATCH /v2/feedbacks/:feedback_id/close`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/20/close"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;cb9962973abe8842d27a4eb0c92e800cfa32b29ea6fcc0b9b7cf995969e0aad9"</code>
## publishes feedbackable

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer 113a9d2b6e8f1de62220bacef8bb9c018508daf5649b8339ee3eb61afe92eb8f
```

`PATCH /v2/feedbacks/:feedback_id/fix`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/26/fix"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;113a9d2b6e8f1de62220bacef8bb9c018508daf5649b8339ee3eb61afe92eb8f"</code>
## removes fields of study ids if an empty array is sent

### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c18b0a8010ae48ebd7df3685856862e545c51151e93f19808464a603c2ac99e0
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
    "id": 257,
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
    "created_at": "2016-06-01T15:50:16.304Z",
    "updated_at": "2016-06-01T15:50:16.304Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-d&nbsp;'{"fields_of_study":[]}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;c18b0a8010ae48ebd7df3685856862e545c51151e93f19808464a603c2ac99e0"</code>
## removes previously set topic if excluded from the list

### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 4872dee7d7f34482ad7f6f34b8ad3c242c72ae917835ee6de7d2a180cb849c29
```

`PATCH /v2/me/user`


#### Parameters


```json
{"fields_of_study":[75]}
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
    "id": 256,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      75
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-01T15:50:16.201Z",
    "updated_at": "2016-06-01T15:50:16.201Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-d&nbsp;'{"fields_of_study":[75]}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4872dee7d7f34482ad7f6f34b8ad3c242c72ae917835ee6de7d2a180cb849c29"</code>
## reports the comment

### Request

#### Endpoint

```
PUT /v2/comments/8/report
Content-Type: application/json
Authorization: Bearer edcf36f8731dca4a24c0a7f87e39ad3619b16306277eb445ed6fc7f709d2d87b
```

`PUT /v2/comments/:comment_id/report`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/8/report"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;edcf36f8731dca4a24c0a7f87e39ad3619b16306277eb445ed6fc7f709d2d87b"</code>
## reports the flashcard

### Request

#### Endpoint

```
PUT /v2/flashcards/58/report
Content-Type: application/json
Authorization: Bearer be5b526811c20aef1752b6bdd7858ddf2309dacc0d5c8ed32412d8d867dd0a06
```

`PUT /v2/flashcards/:flashcard_id/report`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/58/report"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;be5b526811c20aef1752b6bdd7858ddf2309dacc0d5c8ed32412d8d867dd0a06"</code>
## reports the question

### Request

#### Endpoint

```
PUT /v2/questions/3/report
Content-Type: application/json
Authorization: Bearer acab9bef25554ecb3eb997ae638864efe58100103271928bf1972c582cd69461
```

`PUT /v2/questions/:question_id/report`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/3/report"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;acab9bef25554ecb3eb997ae638864efe58100103271928bf1972c582cd69461"</code>
## republishes the comment

### Request

#### Endpoint

```
PUT /v2/comments/6/republish
Content-Type: application/json
Authorization: Bearer caa02ca0728c30681806f05bd20502956a2f34733d17c7a15d63586a94445660
```

`PUT /v2/comments/:comment_id/republish`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/comments/6/republish"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PUT&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;caa02ca0728c30681806f05bd20502956a2f34733d17c7a15d63586a94445660"</code>
## responds with a course

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 4a9a3c245dc5eabf7eab96cf9c83e13a8134db63e40040dd271dc40d5d964ecc
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
    "creator_id": 414,
    "id": 109,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 116,
    "additional_university_ids": [

    ],
    "topic_id": 119,
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
    "chapters_updated_at": "2016-06-01T15:50:44.156Z",
    "updated_at": "2016-06-01T15:50:44.160Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 91,
        "title": "Clever Chapter Title 75",
        "position": 1,
        "updated_at": "2016-06-01T15:50:44.084Z",
        "course_id": 109,
        "author_id": 414,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-01T15:50:43.905Z",
        "questions_updated_at": "2016-06-01T15:50:43.057Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 92,
        "title": "Clever Chapter Title 76",
        "position": 2,
        "updated_at": "2016-06-01T15:50:44.156Z",
        "course_id": 109,
        "author_id": 414,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-01T15:50:44.004Z",
        "questions_updated_at": "2016-06-01T15:50:43.461Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 415,
        "chapter_id": 91,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.835Z",
        "created_at": "2016-06-01T15:50:43.835Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 415,
        "chapter_id": 92,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.942Z",
        "created_at": "2016-06-01T15:50:43.942Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 415,
        "chapter_id": 91,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.905Z",
        "created_at": "2016-06-01T15:50:43.905Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 415,
        "chapter_id": 92,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:44.004Z",
        "created_at": "2016-06-01T15:50:44.004Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ],
    "questions": [
      {
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 415,
        "chapter_id": 91,
        "position": 39,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:42.871Z",
        "created_at": "2016-06-01T15:50:42.806Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
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
        "author_id": 415,
        "chapter_id": 91,
        "position": 40,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.057Z",
        "created_at": "2016-06-01T15:50:42.980Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
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
      },
      {
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 415,
        "chapter_id": 92,
        "position": 41,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.250Z",
        "created_at": "2016-06-01T15:50:43.171Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 104,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 105,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 415,
        "chapter_id": 92,
        "position": 42,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:43.461Z",
        "created_at": "2016-06-01T15:50:43.398Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 106,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 107,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4a9a3c245dc5eabf7eab96cf9c83e13a8134db63e40040dd271dc40d5d964ecc"</code>
## responds with a course

### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 8f53b3628e331a69e2d7e26d6de8818aad74a36cc135d83ce4554c31ea0b761f
```

`GET /v2/courses/:course_slug_or_id`


#### Parameters


```json
include: flashcards, invalid_resources
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
    "creator_id": 408,
    "id": 108,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "topic_id": 118,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 6,
    "questions_count": 6,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": true,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-06-01T15:50:41.905Z",
    "updated_at": "2016-06-01T15:50:41.954Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 89,
        "title": "Clever Chapter Title 73",
        "position": 1,
        "updated_at": "2016-06-01T15:50:41.782Z",
        "course_id": 108,
        "author_id": 408,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-06-01T15:50:41.768Z",
        "questions_updated_at": "2016-06-01T15:50:41.065Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 90,
        "title": "Clever Chapter Title 74",
        "position": 2,
        "updated_at": "2016-06-01T15:50:41.905Z",
        "course_id": 108,
        "author_id": 408,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-06-01T15:50:41.898Z",
        "questions_updated_at": "2016-06-01T15:50:41.212Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 408,
        "chapter_id": 89,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.267Z",
        "created_at": "2016-06-01T15:50:41.267Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 408,
        "chapter_id": 90,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.432Z",
        "created_at": "2016-06-01T15:50:41.432Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 408,
        "chapter_id": 89,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.356Z",
        "created_at": "2016-06-01T15:50:41.356Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 408,
        "chapter_id": 90,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.566Z",
        "created_at": "2016-06-01T15:50:41.566Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 411,
        "chapter_id": 89,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.768Z",
        "created_at": "2016-06-01T15:50:41.768Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 412,
        "chapter_id": 90,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:41.898Z",
        "created_at": "2016-06-01T15:50:41.898Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8f53b3628e331a69e2d7e26d6de8818aad74a36cc135d83ce4554c31ea0b761f"</code>
## responds with a course

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
    "creator_id": 420,
    "id": 110,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 117,
    "additional_university_ids": [

    ],
    "topic_id": 120,
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
    "chapters_updated_at": "2016-06-01T15:50:46.234Z",
    "updated_at": "2016-06-01T15:50:46.243Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 93,
        "title": "Clever Chapter Title 77",
        "position": 1,
        "updated_at": "2016-06-01T15:50:46.126Z",
        "course_id": 110,
        "author_id": 420,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-01T15:50:45.790Z",
        "questions_updated_at": "2016-06-01T15:50:44.736Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 94,
        "title": "Clever Chapter Title 78",
        "position": 2,
        "updated_at": "2016-06-01T15:50:46.234Z",
        "course_id": 110,
        "author_id": 420,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-06-01T15:50:45.917Z",
        "questions_updated_at": "2016-06-01T15:50:45.038Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 420,
        "chapter_id": 93,
        "position": 45,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:44.736Z",
        "created_at": "2016-06-01T15:50:44.682Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
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
      },
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 420,
        "chapter_id": 94,
        "position": 47,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-06-01T15:50:45.038Z",
        "created_at": "2016-06-01T15:50:44.972Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 116,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 117,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;"</code>
## responds with campaign

### Request

#### Endpoint

```
GET /v2/campaigns/1
Content-Type: application/json
Authorization: Bearer a6ea5662155af6f5475a6a6f3b8dec57178f980cae1c2ec61d473ea3058bac94
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
    "company_id": 12,
    "precluded_campaign_ids": [

    ],
    "company_profiles": [

    ],
    "banners": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/campaigns/1"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a6ea5662155af6f5475a6a6f3b8dec57178f980cae1c2ec61d473ea3058bac94"</code>
## responds with chapter

### Request

#### Endpoint

```
GET /v2/chapters/59
Content-Type: application/json
Authorization: Bearer 6dea9249a67f0e8aea6c034750dbc6d2435282778f36b027746b578c082af2fe
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
    "id": 59,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-06-01T15:50:14.367Z",
    "course_id": 66,
    "author_id": 241,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 245,
        "chapter_id": 59,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-06-01T15:50:14.357Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ],
    "questions": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 243,
        "chapter_id": 59,
        "position": 17,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-06-01T15:50:14.147Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 54,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 55,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/59"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;6dea9249a67f0e8aea6c034750dbc6d2435282778f36b027746b578c082af2fe"</code>
## responds with chapter

### Request

#### Endpoint

```
GET /v2/chapters/60
Content-Type: application/json
Authorization: Bearer 03ac40559fc78dc15193ece8e687c320caef5d12448cebb8aadd88b99ef45639
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
    "id": 60,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-06-01T15:50:15.245Z",
    "course_id": 67,
    "author_id": 248,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2015-03-12T14:00:00.000Z",
    "questions_updated_at": "2015-04-12T14:00:00.000Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 251,
        "chapter_id": 60,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T14:00:00.000Z",
        "created_at": "2016-06-01T15:50:15.048Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      },
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 252,
        "chapter_id": 60,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-06-01T15:50:15.232Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
        "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
      }
    ],
    "questions": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 249,
        "chapter_id": 60,
        "position": 18,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T14:00:00.000Z",
        "created_at": "2016-06-01T15:50:14.754Z",
        "tags": [

        ],
        "published": false,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 56,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 57,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 250,
        "chapter_id": 60,
        "position": 19,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-06-01T15:50:14.911Z",
        "tags": [

        ],
        "published": true,
        "reported": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 58,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 59,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/60"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;03ac40559fc78dc15193ece8e687c320caef5d12448cebb8aadd88b99ef45639"</code>
## responds with collection

### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 5b6609ea04fc096aa3c3ead6938b0a9116fdd93e1aa59975d079def995d5b6cb
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
      "creator_id": 189,
      "id": 47,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "topic_id": 52,
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
      "updated_at": "2016-06-01T15:50:08.128Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/search/courses?query=Pi"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5b6609ea04fc096aa3c3ead6938b0a9116fdd93e1aa59975d079def995d5b6cb"</code>
## responds with collection

### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 28aa8d1dc96039eb0380978f4ebf0d8c8052c9ec7fe8055f16fce4a75d1af9e3
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
      "id": 55,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-53",
      "html_url": "https://goskive.com/university/uni-53",
      "slug": "uni-53",
      "name": "National School of Pizza",
      "short_name": "Uni 53",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/f2afd3abe283ce839fc9a384be143562b2b72080.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/86d9dd0868c68816958be02931ecc4e0895c85e7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-01T15:50:08.692Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 54,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-52",
      "html_url": "https://goskive.com/university/uni-52",
      "slug": "uni-52",
      "name": "National School of Pastry",
      "short_name": "Uni 52",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/690013fdb447e68398e079be137a317e0c29574d.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/137c9b9fb39d337e3b136d8aade16f25e8e796d5.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-06-01T15:50:08.656Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/search/universities?query=NSP"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;28aa8d1dc96039eb0380978f4ebf0d8c8052c9ec7fe8055f16fce4a75d1af9e3"</code>
## responds with company

### Request

#### Endpoint

```
GET /v2/companies/24
Content-Type: application/json
Authorization: Bearer cf20dc223c03592543e93c0098bb9c198f64aaaf2affa75cdaa89c6df8d5355f
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
    "id": 24,
    "name": "Pastry Corp",
    "logo_url": null,
    "brand_color": "#ffcc00",
    "updated_at": "2016-06-01T15:51:14.525Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/companies/24"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;cf20dc223c03592543e93c0098bb9c198f64aaaf2affa75cdaa89c6df8d5355f"</code>
## responds with complete user profile

### Request

#### Endpoint

```
GET /v2/users/54
Content-Type: application/json
Authorization: Bearer 5fda9a964c1f3d26945005e209a0048509d7f8d6f0cb047cd01ffe4021daf3b9
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
    "id": 54,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 14,
    "fields_of_study": [
      14,
      15
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-06-01T15:49:34.123Z",
    "updated_at": "2016-06-01T15:49:34.123Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/users/54"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5fda9a964c1f3d26945005e209a0048509d7f8d6f0cb047cd01ffe4021daf3b9"</code>
## responds with discipline and translations

### Request

#### Endpoint

```
GET /v2/disciplines/203
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
    "id": 203,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 203,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 203
      },
      {
        "id": 204,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 203
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/disciplines/203"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## responds with feedback

### Request

#### Endpoint

```
GET /v2/feedbacks/17
Content-Type: application/json
Authorization: Bearer bef5dfccc928f3c8efe848dee148720011a95f9764d2eba72c7f48a0ca741fa4
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
    "id": 17,
    "user_id": 306,
    "feedbackable_id": 25,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-06-01T15:50:24.637Z",
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



### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/17"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;bef5dfccc928f3c8efe848dee148720011a95f9764d2eba72c7f48a0ca741fa4"</code>
## responds with flashcard

### Request

#### Endpoint

```
GET /v2/flashcards/62
Content-Type: application/json
Authorization: Bearer 51aa0e61b11b3ea4df2fc05f430ebef1e65901088a503127c1f0508941529bab
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
    "id": 62,
    "obfuscated_id": "fj_KMGohXD4",
    "author_id": 482,
    "chapter_id": 108,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:50:55.279Z",
    "created_at": "2016-06-01T15:50:55.279Z",
    "tags": [

    ],
    "published": true,
    "reported": false,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
    "back_content_html": "<!doctype html>\n                        <html lang=en>\n                        <head>\n                        <meta charset=utf-8>\n                        <title>A Title</title>\n                        </head>\n                        <body>\n                        <p>I'm the content</p>\n                        </body>\n                        </html>"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/62"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;51aa0e61b11b3ea4df2fc05f430ebef1e65901088a503127c1f0508941529bab"</code>
## responds with minimal user profile

### Request

#### Endpoint

```
GET /v2/users/52
Content-Type: application/json
Authorization: Bearer b654038aeaa0a3d3679f5089ebce385e4242acc3e69f7869bb81194e97f72fbb
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
    "id": 52,
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
    "created_at": "2016-06-01T15:49:32.791Z",
    "updated_at": "2016-06-01T15:49:32.791Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/users/52"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b654038aeaa0a3d3679f5089ebce385e4242acc3e69f7869bb81194e97f72fbb"</code>
## responds with question

### Request

#### Endpoint

```
GET /v2/questions/2
Content-Type: application/json
Authorization: Bearer d1da763f39de48978f00b6804d1b1645fe3d370d5c600a4cb11c9bd98b9f4423
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
    "id": 2,
    "obfuscated_id": "yHhUU9c1C7Y",
    "author_id": 18,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:49:23.330Z",
    "created_at": "2016-06-01T15:49:23.295Z",
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
    "published": true,
    "reported": false,
    "language_code": "de",
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 3,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 4,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/2"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d1da763f39de48978f00b6804d1b1645fe3d370d5c600a4cb11c9bd98b9f4423"</code>
## responds with topic and translations

### Request

#### Endpoint

```
GET /v2/topics/33
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
    "id": 33,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 33
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/topics/33"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## responds with university

### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer d4b27c503f83675a5e2e2be9d36844810c8265d43ac225e5c654149cb2b5f058
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
    "id": 39,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/a7f77c43dfd5ecc00660cdc5a443484d3d65c8a5.png",
    "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/5e2c981db254fae9a6b35d65b5209d2ad371995f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-06-01T15:50:00.805Z",
    "url": "http://www.fu-berlin.de",
    "latitude": "52.496403",
    "longitude": "13.357812",
    "published": true
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/universities/fu-berlin"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d4b27c503f83675a5e2e2be9d36844810c8265d43ac225e5c654149cb2b5f058"</code>
## responds with user

### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer b41fd81255db8a96846f5b37d8b6e10e46fc8c4c88af65c0d7843027766fda5d
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
    "id": 259,
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
    "created_at": "2016-06-01T15:50:17.395Z",
    "updated_at": "2016-06-01T15:50:17.395Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b41fd81255db8a96846f5b37d8b6e10e46fc8c4c88af65c0d7843027766fda5d"</code>
## responds with user course

### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 7b4bb5dfe2da64d2bd3bed48c7d312d54b248ad282f11cdef234301e24340061
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
    "id": 7,
    "course_id": 178,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-06-01T15:51:08.061Z",
    "course_published": true,
    "updated_at": "2016-06-01T15:51:08.047Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses/7"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;7b4bb5dfe2da64d2bd3bed48c7d312d54b248ad282f11cdef234301e24340061"</code>
## responds with vote

### Request

#### Endpoint

```
GET /v2/votes/6
Content-Type: application/json
Authorization: Bearer b18e8fac34318c072a4726e02a7c00f9e0c25bac8ecfaed924ca56b4f693e6c5
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
    "id": 6,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 19,
    "user_id": 177
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/votes/6"&nbsp;-X&nbsp;GET&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b18e8fac34318c072a4726e02a7c00f9e0c25bac8ecfaed924ca56b4f693e6c5"</code>
## sends a password reset email

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





### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"email":"jan.turnosky@hotmail.sk"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## sends a password reset email

### Request

#### Endpoint

```
POST /v2/password
Content-Type: application/json
```

`POST /v2/password`


#### Parameters


```json
{"password":{"email":"jan.meier@hotmail.de"}}
```


| Name | Description |
|:-----|:------------|
| password[email] *required* | Email address |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/password"&nbsp;-d&nbsp;'{"password":{"email":"jan.meier@hotmail.de"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"</code>
## sends an email to feedback author

### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/close
Content-Type: application/json
Authorization: Bearer efaaf884c808c6e3d4091d7d87e740638c6d008f5ce3e82bcd2de0b6578b523b
```

`PATCH /v2/feedbacks/:feedback_id/close`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/22/close"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;efaaf884c808c6e3d4091d7d87e740638c6d008f5ce3e82bcd2de0b6578b523b"</code>
## sends an email to feedback author

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer a971631f572ec3fec2cf901c70ab4e7443c9df2238743e2e714d87724716db4b
```

`PATCH /v2/feedbacks/:feedback_id/fix`


#### Parameters


None known.


### Response

```

204 No Content
```





### cURL

<code>curl&nbsp;"api.goskive.com/v2/feedbacks/25/fix"&nbsp;-d&nbsp;''&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;a971631f572ec3fec2cf901c70ab4e7443c9df2238743e2e714d87724716db4b"</code>
## sends email to the given email address

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 1dc934bab898adeddc6deead2bcfcc05391339d2f75476e3cda353f7deec5ce9
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/jobs/7/sign_ups"&nbsp;-d&nbsp;'{"sign_up":{"email_address":"joe@megacorp.com"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1dc934bab898adeddc6deead2bcfcc05391339d2f75476e3cda353f7deec5ce9"</code>
## signs up the user

### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 8e1ba159f789868cb123153f9fa0273b13d5dc3f24d2616fc95393a7368fb5ec
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
  "created_at": "2016-06-01T15:49:25.381Z",
  "all_access_pass": false,
  "eligible_for_first_course_purchase_discount": false,
  "email": "jan.turnosky@hotmail.cz",
  "display_name": "Jan Turnosky",
  "course_ids": [

  ]
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/users"&nbsp;-d&nbsp;'{"authentication_type":"password","email":"jan.turnosky@hotmail.cz","first_name":"Jan","last_name":"Turnosky","password":"Vykupiteli"}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;8e1ba159f789868cb123153f9fa0273b13d5dc3f24d2616fc95393a7368fb5ec"</code>
## signs up the user with the given email address

### Request

#### Endpoint

```
POST /v2/me/widgets/2/sign_ups
Content-Type: application/json
Authorization: Bearer 4ebafa7532ea6a21c3cd942921203ac9c0989f9118f8549c30cb515862963f13
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/widgets/2/sign_ups"&nbsp;-d&nbsp;'{"sign_up":{"email_address":"joe@megacorp.com"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;4ebafa7532ea6a21c3cd942921203ac9c0989f9118f8549c30cb515862963f13"</code>
## signs up the user with the given email address

### Request

#### Endpoint

```
POST /v2/me/jobs/8/sign_ups
Content-Type: application/json
Authorization: Bearer 5a50f0f22e3990ca1fb5f0e2527ddeed365281949090472fdcd6d69fd7396d98
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/jobs/8/sign_ups"&nbsp;-d&nbsp;'{"sign_up":{"email_address":"joe@megacorp.com"}}'&nbsp;-X&nbsp;POST&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;5a50f0f22e3990ca1fb5f0e2527ddeed365281949090472fdcd6d69fd7396d98"</code>
## unpins the course (update the user course)

### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer b49dfcf6857b1dde6bcae209a1bdcbee6de1442f67f5593d8809279ac7c7fff5
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
    "course_id": 177,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-06-01T15:51:07.873Z",
    "course_published": true,
    "updated_at": "2016-06-01T15:51:07.860Z"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user_courses/6"&nbsp;-d&nbsp;'{"user_course":{"pinned":false}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b49dfcf6857b1dde6bcae209a1bdcbee6de1442f67f5593d8809279ac7c7fff5"</code>
## updates a flashcard

### Request

#### Endpoint

```
PATCH /v2/flashcards/61
Content-Type: application/json
Authorization: Bearer b26b521d210d745dcc686be7d4a31b30585f1a52c779bb981baec45c0231725b
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
    "id": 61,
    "obfuscated_id": "Acd5zhQoy8g",
    "author_id": 479,
    "chapter_id": 107,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:50:55.038Z",
    "created_at": "2016-06-01T15:50:54.614Z",
    "tags": [

    ],
    "published": true,
    "reported": false,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "*rise*",
    "front_content_html": "<!doctype html>\n                         <html lang=en>\n                         <head>\n                         <meta charset=utf-8>\n                         <title>A Title</title>\n                         </head>\n                         <body>\n                         <p>I'm the content</p>\n                         </body>\n                         </html>",
    "back_content_html": "<strong>rise</strong>"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/61"&nbsp;-d&nbsp;'{"flashcard":{"back_content":"*rise*","back_content_html":"&#92;u003cstrong&#92;u003erise&#92;u003c/strong&#92;u003e","language_code":"de"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;b26b521d210d745dcc686be7d4a31b30585f1a52c779bb981baec45c0231725b"</code>
## updates a flashcard with images

### Request

#### Endpoint

```
PATCH /v2/flashcards/60
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 9adfd4b79715b0336ca849c36c79de5a86a1b346959c040189dd4d7bacdbf9e8
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
    "id": 60,
    "obfuscated_id": "XsZtONYAiuo",
    "author_id": 476,
    "chapter_id": 106,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:50:54.291Z",
    "created_at": "2016-06-01T15:50:53.252Z",
    "tags": [

    ],
    "published": true,
    "reported": false,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/466cd80e79a43f1ccb75d4601297e868db9b7c64.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/b1adf22c128fd131c43567d5483bcfad756cdcf6.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/466cd80e79a43f1ccb75d4601297e868db9b7c64.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/b1adf22c128fd131c43567d5483bcfad756cdcf6.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/flashcards/60"&nbsp;-d&nbsp;'------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[front_image]";&nbsp;filename="flashcard_front.jpg"<br>Content-Type:&nbsp;image/jpeg<br>Content-Length:&nbsp;15053<br><br>[uploaded&nbsp;data]<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[back_image]";&nbsp;filename="flashcard_back.jpg"<br>Content-Type:&nbsp;image/jpeg<br>Content-Length:&nbsp;16101<br><br>[uploaded&nbsp;data]<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="flashcard[language_code]"<br><br>de<br>------------XnJLe9ZIbbGUYtzPQJ16u1--'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;multipart/form-data;&nbsp;boundary=----------XnJLe9ZIbbGUYtzPQJ16u1"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;9adfd4b79715b0336ca849c36c79de5a86a1b346959c040189dd4d7bacdbf9e8"</code>
## updates a question

### Request

#### Endpoint

```
PATCH /v2/questions/4
Content-Type: application/json
Authorization: Bearer 59b1f3cb3f13b4e9191960d18d046d114d06cf3b850e4a8340dffc78af4aa428
```

`PATCH /v2/questions/:question_id`


#### Parameters


```json
{"question":{"question":{"id":4,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-06-01T15:49:24.810Z","updated_at":"2016-06-01T15:49:24.847Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":8,"author_id":24,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 24,
    "chapter_id": 8,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-06-01T15:49:24.962Z",
    "created_at": "2016-06-01T15:49:24.810Z",
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
    "published": true,
    "reported": false,
    "language_code": "de",
    "question": "{\"id\"=>4, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-06-01T15:49:24.810Z\", \"updated_at\"=>\"2016-06-01T15:49:24.847Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>8, \"author_id\"=>24, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 7,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 8,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 9,
        "position": 3,
        "content": "Choux needs baking powder.",
        "content_html": "<p>Choux needs baking powder.</p>",
        "correct": false
      }
    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/questions/4"&nbsp;-d&nbsp;'{"question":{"question":{"id":4,"position":1,"type":0,"question":"Clever&nbsp;example&nbsp;question:&nbsp;why&nbsp;did&nbsp;the&nbsp;rspec&nbsp;test&nbsp;not&nbsp;pass?","created_at":"2016-06-01T15:49:24.810Z","updated_at":"2016-06-01T15:49:24.847Z","more":"This&nbsp;could&nbsp;never&nbsp;explain&nbsp;why&nbsp;it&nbsp;didn&#92;u0027t&nbsp;pass.&nbsp;Maybe&nbsp;it&nbsp;did?","chapter_id":8,"author_id":24,"question_html":"&#92;u003cp&#92;u003eClever&nbsp;example&nbsp;question:&nbsp;why&nbsp;did&nbsp;the&nbsp;rspec&nbsp;test&nbsp;not&nbsp;pass?&#92;u003c/p&#92;u003e","more_html":"&#92;u003cp&#92;u003eThis&nbsp;could&nbsp;never&nbsp;explain&nbsp;why&nbsp;it&nbsp;didn&#92;u0027t&nbsp;pass.&nbsp;Maybe&nbsp;it&nbsp;did?&#92;u003cp&#92;u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs&nbsp;do&nbsp;all&nbsp;the&nbsp;work","answer_options":[{"content":"Choux&nbsp;needs&nbsp;baking&nbsp;powder.","content_html":"&#92;u003cp&#92;u003eChoux&nbsp;needs&nbsp;baking&nbsp;powder.&#92;u003c/p&#92;u003e","correct":false}]}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;59b1f3cb3f13b4e9191960d18d046d114d06cf3b850e4a8340dffc78af4aa428"</code>
## updates a vote

### Request

#### Endpoint

```
PATCH /v2/votes/7
Content-Type: application/json
Authorization: Bearer fc7833eebbcedf8bfd4817dedea765faea95cb9f02356a68076fcae817467ac5
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
    "id": 7,
    "type": "DownVote",
    "votable_type": "Question",
    "votable_id": 20,
    "user_id": 181
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/votes/7"&nbsp;-d&nbsp;'{"vote":{"type":"DownVote"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;fc7833eebbcedf8bfd4817dedea765faea95cb9f02356a68076fcae817467ac5"</code>
## updates current user

### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d484ecd643dca2a17f31ec1d52ddb3d6c0447c56956ee8a5edcd561c2ef905b7
```

`PATCH /v2/me/user`


#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[73]}
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
    "id": 254,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      73
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-01T15:50:15.752Z",
    "updated_at": "2016-06-01T15:50:15.886Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-d&nbsp;'{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[73]}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;d484ecd643dca2a17f31ec1d52ddb3d6c0447c56956ee8a5edcd561c2ef905b7"</code>
## updates current user with an image

### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer e1397422af4947fb86e33e03499b10ee13a497ece73e12e1345ba0994fdb73f2
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

77
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
    "id": 258,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/thumb/6bc4583231a77a013ef10dac99c1f1167e855136.jpg",
    "university_id": null,
    "fields_of_study": [
      77
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-06-01T15:50:16.610Z",
    "updated_at": "2016-06-01T15:50:17.244Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/orginal/4fb4d471748379bc639cdd120dc4a7ee1fefa86d.jpg",
    "course_ids": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/user"&nbsp;-d&nbsp;'------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="email"<br><br>magnus@gmail.sk<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="first_name"<br><br>Sven<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="fields_of_study[]"<br><br>77<br>------------XnJLe9ZIbbGUYtzPQJ16u1<br>Content-Disposition:&nbsp;form-data;&nbsp;name="image";&nbsp;filename="contact_avatar.jpg"<br>Content-Type:&nbsp;image/jpeg<br>Content-Length:&nbsp;12418<br><br>[uploaded&nbsp;data]<br>------------XnJLe9ZIbbGUYtzPQJ16u1--'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;multipart/form-data;&nbsp;boundary=----------XnJLe9ZIbbGUYtzPQJ16u1"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e1397422af4947fb86e33e03499b10ee13a497ece73e12e1345ba0994fdb73f2"</code>
## updates permitted course properties

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 774581b5c8df1f526563005ebdd3a33afe517625d0b4794da0f4d9dfe33777fe
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
    "creator_id": 381,
    "id": 97,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 104,
    "additional_university_ids": [

    ],
    "topic_id": 107,
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
    "updated_at": "2016-06-01T15:50:34.202Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;102","language_code":"fr","published":false}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;774581b5c8df1f526563005ebdd3a33afe517625d0b4794da0f4d9dfe33777fe"</code>
## updates permitted course properties

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e0e6080d512a482fbf17cf07eb01ca20daf3ce79854dad5bbf855d93d615795f
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
    "creator_id": 379,
    "id": 96,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 106,
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
    "user_generated": false,
    "published": false,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-06-01T15:50:33.849Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/courses/fu-choux-pastry-101"&nbsp;-d&nbsp;'{"course":{"title":"Choux&nbsp;pastry&nbsp;102","language_code":"fr","published":false}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;e0e6080d512a482fbf17cf07eb01ca20daf3ce79854dad5bbf855d93d615795f"</code>
## updates the chapter

### Request

#### Endpoint

```
PATCH /v2/chapters/53
Content-Type: application/json
Authorization: Bearer 149c218a95ddd639727641d759d2ec3a00085d047928ca36d98a8ec6d64fb206
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
    "id": 53,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-06-01T15:50:11.864Z",
    "course_id": 60,
    "author_id": 224,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/53"&nbsp;-d&nbsp;'{"chapter":{"title":"Eggs&nbsp;and&nbsp;Flour"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;149c218a95ddd639727641d759d2ec3a00085d047928ca36d98a8ec6d64fb206"</code>
## updates the chapter

### Request

#### Endpoint

```
PATCH /v2/chapters/54
Content-Type: application/json
Authorization: Bearer 1ed2a15e047091e4d622c81242aab6c8c41d69a6e3e6ec69d9449ced8504b3df
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
    "id": 54,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-06-01T15:50:12.204Z",
    "course_id": 61,
    "author_id": 226,
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




### cURL

<code>curl&nbsp;"api.goskive.com/v2/chapters/54"&nbsp;-d&nbsp;'{"chapter":{"title":"Eggs&nbsp;and&nbsp;Flour"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;1ed2a15e047091e4d622c81242aab6c8c41d69a6e3e6ec69d9449ced8504b3df"</code>
## updates the notification

### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer 2e166b17ee83b7a6de602e5be6ed094ad756e80b3635951fa13e63f913b04a77
```

`PATCH /v2/me/notifications/:notification_id`


#### Parameters


```json
{"notification":{"read_at":"2016-06-01T15:40:46.000Z"}}
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
    "id": 14,
    "created_at": "2016-06-01T15:50:46.697Z",
    "read_at": "2016-06-01T15:40:46.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 14,
    "updated_at": "2016-06-01T15:50:46.873Z",
    "author_id": "427",
    "thread_subject_id": "111",
    "thread_subject_type": "Course"
  }
}
```




### cURL

<code>curl&nbsp;"api.goskive.com/v2/me/notifications/14"&nbsp;-d&nbsp;'{"notification":{"read_at":"2016-06-01T15:40:46.000Z"}}'&nbsp;-X&nbsp;PATCH&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Content-Type:&nbsp;application/json"&nbsp;&#92;<br>&nbsp;&nbsp;-H&nbsp;"Authorization:&nbsp;Bearer&nbsp;2e166b17ee83b7a6de602e5be6ed094ad756e80b3635951fa13e63f913b04a77"</code>
