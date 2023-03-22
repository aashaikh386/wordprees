sudo apt update -y
sudo apt install nginx -y
sudo systemctl start nginx
sudo systemctl status nginx (check on browser that nginx is working or not)
sudo apt install mysql-server mysql-client -y
sudo systemctl start mysql
sudo systemctl status mysql
sudo systemctl enable mysql
sudo systemctl enable nginx
sudo mysql_secure_installation
	y
	2
	Vishal@135
	Vishal@135
	y
	y
	y
	y
	y
sudo mysql -u root -p
	Alex@135
create database wordpress;
CREATE USER 'wp_user'@localhost IDENTIFIED BY 'Mysql@sql135';
GRANT ALL PRIVILEGES ON wordpress.* TO 'wp_user'@localhost;
flush privileges;
exit;
sudo apt install php php-gd php-mysql php-zip php-fpm -y
wget https://wordpress.org/latest.zip
sudo apt install unzip -y
unzip latest.zip
cd wordpress/
sudo cp -r * /var/www/html/
sudo chown -R www-data:www-data /var/www/html/
sudo systemctl restart nginx
cd /etc/nginx/sites-enabled/ 
ls
sudo mv default wordpress
ls
sudo nano wordpress
	
sudo systemctl restart nginx
sudo nginx -t (ok & successful)
sudo systemctl restart nginx# wordprees
