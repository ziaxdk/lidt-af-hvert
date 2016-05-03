# Containers

## Pre install

```
docker run -d --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=somepass mysql:5.7.12
docker run -d --name presta -p 8080:80 --link mysql:mysql prestashop/prestashop:1.6.1.5
```

## Post install

```
docker exec -it presta bash
rm -rf install
mv admin admin-shop
```

# Start

```
http://192.168.99.100:8080
http://192.168.99.100:8080/admin-shop
```
