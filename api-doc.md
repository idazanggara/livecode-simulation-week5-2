# baby-factory-server

​
List of available endpoints:
​
- `POST /register`
- `POST /login`

And routes below need authentication
- `POST /babies`
- `GET /babies`
- `DELETE /babies/:id`

### POST /register

Request:

- data:

```json
{
  "email": "string",
  "password": "string"
}
```

Response:

- status: 201
- body:
  ​

```json
{
  "id": "integer",
  "email": "string"
}
```

### POST /login

Request:

- data:

```json
{
  "email": "string",
  "password": "string"
}
```

Response:

- status: 200
- body:
  ​

```json
{
  "access_token": "string"
}
```

### POST /babies
Request:

- headers: access_token

- data:

```json
{
  "name": "Jane Doe",
  "img": "https://images.unsplash.com/photo-1511852365831-4c1b2b2b1325?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80"
}
```

​Response:

- status: 201
- body:
  ​

```json
{
  "id": "integer",
  "UserId": "integer",
  "name": "string",
  "img": "string"
}
```

### GET /babies

Description: Get all current logged in user babies

Request:

- headers:
  - access_token: string

Response:

- status: 200
- body:
  ​

```json
[
  {
      "id": "integer",
      "name": "string",
      "img": "string",
      "UserId": "integer",
      "createdAt": "2020-04-17T05:45:10.669Z",
      "updatedAt": "2020-04-17T05:45:10.669Z"
  },{
    ...
  }
]
```

### DELETE /babies/:id

description: 
  Delete one of the current logged in user babies. (cannot delete another user babies use authorization)

Request:

- headers: access_token
- params: 
  - id: integer (required)

Response:

- status: 200
- body:

```json
{
    "message": "Delete babies successfull"
}
```
