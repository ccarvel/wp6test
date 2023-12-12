# README
This is mostly the official WordPress Docker [repo](https://github.com/docker-library/wordpress) with modifications to their [PHP8.1 Dockerfile](https://github.com/docker-library/wordpress/blob/ac65dab91d64f611e4fa89b5e92903e163d24572/latest/php8.1/fpm/Dockerfile) to install git, curl, and wget into the WordPress container.

In addition to the slight mods to the Dockerfile, I have created a docker-compose.yml file that adds a phpMyAdmin service in addition to WordPress and MySQL.

**Versions**  
Versions of these images are:  
WordPress 6.4.2 with PHP 8.1  
MySQL 5.7  
phpMyAdmin 5.2.1  

**Running**   
To run, install and start Docker Desktop;  
Clone or Fork this repo;  
Enter its directory in Terminal;  
run: 
```
docker-compose up -d
```

**Container Names and Entering**  
Containers are named and include their version numbers:   
wp642 (WordPress)  
mysql57 (MySQL)   
phpmyadmin521 (phpMyAdmin)

To enter those containers simply execute
```
docker exec -it [containername] bash
```
eg
```
docker exec -it wp642 bash
```

