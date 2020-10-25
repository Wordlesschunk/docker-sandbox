# docker-sandbox
Simple sandbox container to develop web apps on

to create the container -> docker-compose -d
to stop the container -> docker-compose down
to start the container -> docker-compose up -d

to connect to a service -> docker exec -it [nameOfService] bash

connecting my mysql once within the service -> mysql -u root -p

this container image is meant to be used on local and not on production.

changes coming soon. 



It includes the following:

NGINX
port 8080
PHP
FPM configured for NGINX
XDebug connecting to the docker host
place .php files into a directory named "code" for them to be executable
sendmail
MailDev
you might want to adjust the root mail address in Dockerfile:17
port 8081
MySQL
you also might want to adjust the default password (which is "password") in docker-compose.yml
port 3306
phpmyadmin
defaults see docker-compose.yml, also consider changing the password here too
port 8082


