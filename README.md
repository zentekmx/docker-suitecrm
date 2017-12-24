# SuiteCRM Docker Image

This image provides a SuiteCRM Server. The image is based on php:apache docker image. It depends of a mysql database.

Features
 - Ready to launch with database
 - Exposed volumes
 - Image size of ~800MB

# Usage
```bash
docker pull zentekmx/openldap
docker run -d --name mysqldb -e MYSQL_ROOT_PASSWORD=secret -e MYSQL_DATABASE=suitecrm mysql:5.7
docker run -d -p 80:80 --link mysqldb zentekmx/suitecrm
```

# Exposed ports
 * 80

# Exposed volumes
 * /var/www/html/upload
 * /var/www/html/conf.d

