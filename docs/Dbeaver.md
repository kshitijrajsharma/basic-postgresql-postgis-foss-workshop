## Dbeaver Setup 

DBeaver Community is a free cross-platform database tool for developers, database administrators, analysts, and everyone working with data. It supports all popular SQL databases like MySQL, MariaDB, PostgreSQL, SQLite, Apache Family, and more. You can other database tool like [pgAdmin](https://www.pgadmin.org/) 

## Initial configuration 

After starting your docker container your dbeaver will be available at : http://localhost:8080/ 

- Hit endpoint where dbeaver is running i.e. 8080 port from docker-compose 

    ![Alt text](./img/image.png)

- Click on Next and navigate to ADMINISTRATOR CREDENTIALS

    ![Alt text](./img/image-1.png)

- Setup your login and password & Hit Next

    Mindful to remember this, You will be using it when you login to dbeaver next time 

- Hit Finish 
    ![Alt text](./img/image-2.png)

- After finish you will be promoted to enter your username and password that you created earlier

    ![Alt text](./img/image-3.png)

- Once you are logged in you will see following screen click on top left icon

    ![Alt text](./img/image-4.png)

- This is your query section where you would be instatntiating connections , Shoot query and visualize 

    ![Alt text](./img/image-5.png)


## Connection and Query 

- Click on + Icon on top left bar , Hit New Connection

![Alt text](./img/image-6.png)

- Choose Postgresql , you can use other connections as well such as duckdb 

![Alt text](./img/image-7.png)

- Configure following : 

Those configurations are from docker compose, You can change these to your local if you have any 
```
Host : postgis-docker
User Name : myuser
Password : mypassword
```
![Alt text](./img/image-9.png)

- Fill above in the form box & Hit Test , You should be promoted following box

![Alt text](./img/image-8.png)

- Now finally hit Create ! 

- Expand your connections which will be in left side of your screen , you should be able to see pokhara table 

![Alt text](./img/image-10.png)

### Queries

- Click on SQL button on top left bar , You will be promoted to Query window . Where we will be playing with our data . Click on Select connection and choose your postgis-docker connection

