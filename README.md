# LAMP
Web-based application development using Linux (Debian-10), Apache2 (HTTP Server), MarianDB (MySQL Database), and .PHP scripting.

Here's a great tutorial for setup: https://linuxhint.com/debian_10_lamp_php_dev/  
Here's the command list to set up the LAMP:  

sudo apt update  
sudo apt install mariadb-server mariadb-client  
systemctl status mariadb  
sudo mysql_secure_installation
sudo mysql -u root -p
CREATE DATABASE app1;
GRANT ALL ON app1.* to 'requin'@'localhost' IDENTIFIED BY '123';
FLUSH PRIVILEGES;
sudo apt install apache2 php
sudo systemctl status apache2
sudo apt search ^php-
sudo apt install php-curl php-gd php-mbstring php-mysql php-zip php-json php-xml
sudo systemctl restart apache2
ls /etc/apache2/mods-available
sudo a2enmod rewrite
sudo a2query -m 
sudo nano /etc/apache2/envvars
sudo chown -Rf $(whoami):$whoami) /var/www/html
sudo systemctl restart apache2
