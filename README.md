# Conazon

This is a wrapper monorepo for the conazon project. It pulls all the pieces of the conazon project into one place for simplicity when testing the whole project or making project-wide changes.

This project requires a .env file configured as follows:

```
REACT_APP_PROTOCOL=http
REACT_APP_DOMAIN=localhost
```

and a .env.backend

```
JWTSECRET
CLIENTID
CLIENTSECRET
REDIRECTURL
DATABASEURL='host=postgres port=5432 user=postgres dbname=conazon sslmode=disable'
SECURECOOKIE
```

Run `docker-compose up` to run the project. All other `conazon` back-end endpoints must be running for the project to work