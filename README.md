# Spring Data Rest sample

## mysql server

```
$ docker run --name mysqld -e MYSQL_ROOT_PASSWORD=<ROOT_PASSWORD> -d -p 13306:3306 mysql:5.7
```

## mysql client

```
$ docker run --rm -it --link mysqld:mysqld mysql:5.7 mysql -h mysqld -u root -p
```
