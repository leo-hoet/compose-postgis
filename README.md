# PostGis & PgAdmin4 powered by compose
Forked from [compose-postgres](https://github.com/khezen/compose-postgres)

This compose store postgres data and pgadmin data in new folders inside the root folder

You may need to execute `sudo chown -R 5050:5050 pgadmin` inside the root forder so pgadmin can store its data.

## Requirements:
* docker >= 17.12.0+
* docker-compose

## Quick Start
* Clone or download this repository
* Go inside of directory,  `cd compose-postgis`
* Run this command `docker-compose up -d`


## Environments
This Compose file contains the following environment variables:

* `POSTGRES_USER` the default value is **postgres**
* `POSTGRES_PASSWORD` the default value is **changeme**
* `PGADMIN_PORT` the default value is **5050**
* `PGADMIN_DEFAULT_EMAIL` the default value is **pgadmin4@pgadmin.org**
* `PGADMIN_DEFAULT_PASSWORD` the default value is **admin**

You can create a `.env` file that store the value of enviorment variables like this:
```
POSTGRES_USER=yourUser
POSTGRES_PASSWORD=yourPassword
PGADMIN_DEFAULT_EMAIL=name@domain.com
PGADMIN_DEFAULT_PASSWORD=password
```


## Access to postgres: 
* `localhost:5432`
* **Username:** postgres (as a default)
* **Password:** changeme (as a default)

## Access to PgAdmin: 
* **URL:** `http://localhost:5050`
* **Username:** pgadmin4@pgadmin.org (as a default)
* **Password:** admin (as a default)
