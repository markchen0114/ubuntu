# ubuntu

## Install (Global)
* sudo apt-get update
* sudo apt-get install apache2
* sudo apt-get install cron
* service cron start
* service cron status
---
* sudo apt-get install mysql-server
* sudo mysql_secure_installation
---
* sudo apt-get install php
* sudo apt-get install curl
* curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer
  (install composer globally)
* sudo apt-get install git
* sudo apt-get install npm
* sudo apt-get install php-xml
* sudo apt-get install php-mbstring
* sudo apt-get install php-mysql
* sudo apt-get install php-curl
* sudo npm install -g npm
* sudo npm install -g n
* sudo apt-get install gulp
* sudo npm install npm@latest -g
* apt-get dist-upgrade
---
* a2enmod php7.x
* php artisan cache:clear
* php artisan config:clear
* php artisan view:clear

## Install (Project)
* sudo su
* php artisan passport:install
* npm install -g gulp
* n stable
* sudo npm install --unsafe-perm=true
* sudo chmod 777 -R .git
* sudo apt-get install libpng-dev
* composer install
* npm rebuild node-sass
* nodejs node_modules/node-sass/scripts/install.js
* npm cache clean --force
* sudo npm install natives
* sudo npm install graceful-fs
* php artisan sitemap:generate
* php artisan queue:work --daemon --quiet --queue=default --delay=3 --sleep=3 --tries=3
* sudo npm install --unsafe-perm -g node-sass
* node node_modules/optipng-bin/lib/install.js
* npm upgrade lodash (fix lodash security issue)

* Event & Listener
https://infylife.wordpress.com/2016/08/10/storing-logging-login-activity-in-laravel-application/

## Version
* php --version
* mysql --version
* composer --version
* git --version
* npm --version

## Git
* local git sync from remote
1. git pull
2. git reset --hard HEAD^2
