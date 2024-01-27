# basic-postgresql-postgis-foss-workshop
Basic Postgresql Postgis Workshop

## Prerequisites 

- Postgresql with Postgis enabled 
- Dbeaver / PG Admin 

## Installation 

According to your operating system, Installation differs . You can follow manual install section for that. For this exercise we will install everything with docker which is relatively easy

### Manual install

- Install postgresql in your system : https://www.postgresql.org/download/
- Install postgis : https://postgis.net/workshops/postgis-intro/installation.html 
- Install Dbeaver/ PG Admin : https://dbeaver.io/download/
- Load sample data 
    ``` bash
    psql -a -f data/sql/pokhara.sql
    ```

### Install using Docker 

Install docker in your system. [Get Docker](https://docs.docker.com/get-docker/) 

Once you have docker, Clone this repo & navigate
``` bash
git clone https://github.com/kshitijrajsharma/basic-postgresql-postgis-foss-workshop.git
```
```bash
cd basic-postgresql-postgis-foss-workshop
```
Install and swamp up your containers 

``` bash
docker compose up 
```

Note : Postgresql and dbeaver will loose its state when you cancel your terminal. For persistent usage follow docker instructions about swamping up containers and stuff

## Dbeaver Configuration 

Once you have docker containers running, You can go ahead and [configure Dbeaver](./docs/Dbeaver.md) . We are using dbeaver for this workshop to interact with postgresql tables

## Query 

After dbeaver configuration, You are ready to play with the data. Navigate to [query](./docs/Query.md)


## Resources : 

- Run dbeaver in  docker : https://dbeaver.com/docs/cloudbeaver/Run-Docker-Container/
- Run postgis in docker : https://postgis.net/documentation/getting_started/install_docker/ 
- Postgresql Documentation : https://www.postgresql.org/docs/
- Postgis Documentation : https://postgis.net/documentation/

## Contributions 

Contributions are highly appreciated ! You can enhance this tutorial for workshop or use it in your own ! Feel free to raise PR with your changes 