## Register User

EndPoint : POST /api/v1/auth/register

Request Body :

```json
{
  "username" : "sukriyatma",
  "password" : "matamu",
  "name"     : "Muhammad Sukriyatma" 
}
```

Response Body (success) :

```json
{
  "status"  : "OK",
  "code"    : 200,
  "data"    : {
    "username"  : "sukriyatma",
    "name"      : "Muhammad Sukriyatma"
  }
}
```

Response Body (Failed, 400) :

```json
{
  "status"  : "Bad Request",
  "code"    : 400,
  "errors"  : "Username is required"
}
```

## Login User

EndPoint : POST /api/v1/auth/login

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
    "token" : "token123"
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