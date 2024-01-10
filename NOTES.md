# Notes

## Using a routing third part

* In terminal

``
go get -u github.com/go-chi/chi/v5
``

* To test FRONT and BACK in the same machine, it's necessary to enable CORS middleware.

## Postgres

* Installing driver for postgres = pgx

``
go get github.com/jackc/pgx/v4 &&
go get github.com/jackc/pgconn
``

## JWT

* It's necessary to use third party packages 

``
go get -u github.com/golang-jwt/jwt/v4
``

* It's possible to use with public and private Key but in this code, the JWT is more simple.
  
* Create an account in www.themoviedb.org

## GraphQL

* Use third part

``
go get github.com/graphql-go/graphql
``

## Production

* Change middleware.go
* In mac and linux servers:

``
CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -o gomovies ./cmd/api
``

* A file called 'gomovies' will be created

### Database

``
pg_dump --no-owner -h localhost -p 5432 -U postgres movies > movies.sql
``

## WebServer Production

https://caddyserver.com
https://nginx.org/en/

* Inside ubuntu server

``
sudo apt search supervisor
``

`
sudo apt install supervisor
`

* After see how to install caddy
* Use SCP like a upload files

`
scp build.tgz user@url:/home/folder
`

