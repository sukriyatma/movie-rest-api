# User API Spec

## Current User

EndPoint : GET /api/v1/user/current

Header : 

- Authorization : TOKEN

Response Body (success) :

```json
{
  "status"  : "OK",
  "code"    : 200,
  "data"    : {
    "username"  : "sukriyatma",
    "name"      : "Muhammad Sukriyatma", 
    "token"     : "token123"
  }
}
```

Response Body (Failed) :

```json
{
  "status"  : "Unauthorized",
  "code"    : 401
}
```

## Update User

EndPoint : PATCH /apiv1//user/{id}

Header :

- Authorization : TOKEN

Request Body :

```json
{
  "username" : "sukriyatma",
  "password" : "matamu" 
}
```

Response Body (success) :

```json
{
  "status"  : "OK",
  "code"    : 200,
  "data"    : {
    "token"   : "token123"
  }
}
```

Response Body (Failed, 401) :

```json
{
  "status"  : "Not Found",
  "code"    : 401,
  "errors"  : "Username and Password not match"
}
```

## Logout User

EndPoint : DELETE /api/v1/auth/logout

Header :

- Authorization : TOKEN

Response Body (success) :

```json
{
  "status"  : "OK",
  "code"    : 200
}
```