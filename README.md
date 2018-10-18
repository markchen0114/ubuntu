# ubuntu - Test to Lab

## Install (Global)
* sudo apt-get update
* sudo apt-get install apache2
---
* sudo apt-get install mysql-server
* sudo mysql_secure_installation
---
* sudo apt-get install php
* sudo apt-get install curl
* curl -sS https://getcomposer.org/installer | sudo php -- --install-dir=/usr/local/bin --filename=composer
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
---
* a2enmod php7.x
* php artisan cache:clear

## Install (Project)
* sudo su
* 
* npm install -g gulp
* n stable
* sudo npm install --unsafe-perm=true
* sudo chmod 777 -R .git
* composer install
* npm rebuild node-sass
* nodejs node_modules/node-sass/scripts/install.js
* sudo npm install natives
* sudo npm install graceful-fs
* php artisan queue:work --daemon --quiet --queue=default --delay=3 --sleep=3 --tries=3

## Version
* php --version
* mysql --version
* composer --version
* git --version
* npm --version

## Git
* local git sync from remote
1. git pull
2. git reset --hard HEAD^X -> your branch is ahead of 'branchName' by X commits
