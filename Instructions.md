# Auth server

<!--toc:start-->

- [Auth server](#auth-server)
  - [Installing nestj](#installing-nestj)
  - [Create nestjs project](#create-nestjs-project)
  - [Installing MySQL](#installing-mysql)
  - [Docker container MySQL](#docker-container-mysql)
  <!--toc:end-->

## Installing nestj

`npm i -g @nestjs/cli`

## Create nestjs project

`nest create auth-nestjs`

## Installing MySQL

`npm i --save @nestjs-typeorm typeorm mysql2`

## Docker container MySQL

`docker pull mysql`
`docker run --name mysql-container -e MYSQL_ROOT_PASSWORD=myrootpassword -e MYSQL_DATABASE=auth -e MYSQL_USER=user -e MYSQL_PASSWORD=password123 -p 3306:3306 -d mysql`
`docker ps`
`docker exec -it mysql-container /bin/bash`
`mysql -u root -p`

```sql
SHOW DATABASES;
```

