# TestMysqlDocker
Short test of creating databse and exporting it with docker

## How to use it

1) Download this repo or pull it or clone it.
2) Open a terminal and go to this repertory
3) Execute this command to create a docker image:
```docker build -t mysqlimg . ```
You can replace *mysqlimg* by the name you want to give to this image

4) Execute this command to create and run your docker container:
``` docker run --name=mysqlcont --publish 6603:3456 mysqlimg```
You can replace *mysqlcont* by the name you want to give to this container
You can replace 6603 by any other port, but you need to keep 3456.

You did it. Now you are in mysql into the docker container with the database "greta" and some data already inserted
