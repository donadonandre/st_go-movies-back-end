# Using a routing third part

* In terminal

``
go get -u github.com/go-chi/chi/v5
``

* To test FRONT and BACK in the same machine, it's necessary to enable CORS middleware.

# Postgres

* Installing driver for postgres = pgx

``
go get github.com/jackc/pgx/v4 &&
go get github.com/jackc/pgconn
``

# JWT

* It's necessary to use third party packages 

``
go get -u github.com/golang-jwt/jwt/v4
``