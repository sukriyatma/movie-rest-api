# Movie API Spec

## Add Movie
Method : POST

Endpoint : api/v1/movie

```json
{
    "name" : "",
    "poster" : "",
    "overview" : "",

}
```

## Update Movie
Method : PATCH

Endpoint : api/v1/movie/{id_movie}



## Find Movie by ID
Method : GET

Endpoint : api/v1/movie/{id_movie}

Response : 
```json
{
    "id" : "",
    "name" : "",
    "poster" : "",
    "overview" : "",
    "details" : {
        "title" : "",
        "adult" : false,
        "language" : "",
        "overview" : "",
        "views" : 0,
        "views_today" : 0, 
        "release_date" : "",
        "vote_average" : 0,
        "vote_count" : 0
    }    
}
```



## Search Movies
Method : GET

Endpoint : api/v1/movies/{keyword}



------------------------------------------------

## Get Views
Method : GET

endpoint : api/v1/movie/{id movie}/views

## Get Views Today
Method : GET

endpoint : api/v1/movie/{id movie}/views/today


------------------------------------------------
## Add Favourite Movie
Method : POST

Endpoint : api/v1/movie/{id_movie}/fav


## Delete Favorite Movie 
Method : DELETE

Endpoint : api/v1/movie/{id_movie}/fav


-----------------------------------------------
## Get Release Date
Method : GET

Endpoint : api/v1/movie/{id_movie}/release



----------------------------------------------
## Add Watchlist Movie
Method : POST

Endpoint : api/v1/movie/{id_movie}/watchlist

## Delete Watchlist Movie
Method : POST

Endpoint : api/v1/movie/{id_movie}/watchlist
