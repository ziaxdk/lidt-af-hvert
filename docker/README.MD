# MySql

```
docker run -d --name mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=somepass mysql:5.7.12
```

# PrestaShop

```
docker run -d --name presta -p 8080:80 --link mysql:mysql prestashop/prestashop:1.6.1.5
```


