# MySQL

Starting a MySQL server image:

```
docker pull mysql
docker run --name mysql MYSQL_ROOT_PASSWORD=root  MYSQL_DATABASE=dev -p 3306:3306 mysql
```