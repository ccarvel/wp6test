# README
This is a Dockerfile with a PHP8.2-FPM base to build WordPress, which can be accomplished with the docker-compose.yml file here.

In addition to the slight mods to the Dockerfile (additional installations of git, wget, curl), I have created a docker-compose.yml file that uses Nginx to serve the WordPress content and adds MySQL and phpMyAdmin services.

**Versions**  
Versions of these images are:  
WordPress 6.4.2 with PHP 8.2-FPM  
MySQL 5.7  
phpMyAdmin 5.2.1
Nginx 1.25.3

**Running**   
To run, install and start Docker Desktop;  
Clone or Fork this repo;  
Enter its directory in Terminal;  
run: 
```
docker-compose up -d
```
To verify the WordPress container is successfully running, open a browser and visit:   
```
http://localhost
```
From there you should be able to install WordPress. 

**Container Names and Entering**  
Containers are named and include their version numbers:   
wp642 (WordPress)  
mysql57 (MySQL)   
phpmyadmin521 (phpMyAdmin)   
nginx1253 (Nginx)   


To enter those containers simply execute
```
docker exec -it [containername] bash
```
eg
```
docker exec -it wp642 bash
```

