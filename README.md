# Arazcloud-Tasks
## Task-1
In this task, i should run one WordPress application on the test server and change the default WordPress database to Postgresql database then change the   default web-server to Nginx web-server.
### install wordpress and configure Apache
install wordpress and configure Apache from this [link](https://ubuntu.com/tutorials/install-and-configure-wordpress#3-install-wordpress) .
### install PS4WP
`cd srv/www/wordpress/wp-content` and clone  `git clone https://github.com/kevinoid/postgresql-for-wordpress.git` 
create database/username/password and grant all together.
### Connect PS4WP
`sudo -u www-data cp /srv/www/wordpress/wp-config-sample.php /srv/www/wordpress/wp-config.php` and add data base details to wp-config.php file.
Rename Pg4wp to pg4wp ( also you can ‘nano db.php’ to understand name of directory you should mv Pg4wp ).
### Nginx and Certificate
Down apache service and `Cd etc/nginx/sites-available`  open defualt to configure nginx.
for ssl certificate `sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/private/apache.key -out /etc/ssl/certs/apache.crt`
install  install php7.4-fpm .
reload nginx and check result.
## Task-2
In this task first you should touch one html file with green background.
`touh index.html`
`
<!DOCTYPE html>
<html>
<body style="background-color:#008000;">

<h1>No Problme every thing will be OK </h1>

</body>
</html>
`
