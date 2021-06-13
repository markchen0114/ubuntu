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
* cross-env sass-load lib-dev 這幾個套件，在 apt 及 npm 要先裝好, 沒裝好直接 npm install 後面都會裝不起來

* Event & Listener
https://infylife.wordpress.com/2016/08/10/storing-logging-login-activity-in-laravel-application/

* apache2
/etc/apache2/site-available/laravel.conf
```
<VirtualHost *:80>
    ServerName dev1on1.ltd
    
    ServerAdmin webmaster@localhost
    DocumentRoot /var/www/html/dev1on1/public
    
    <Directory /var/www/html/dev1on1>
        AllowOverride All
    </Directory
    
    ErrorLog ${APACHE_LOG_DIR}/error.log
    CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>
```

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
3. git remote -v

在原本的 1on1 用 remote add 就可以推了
* git remote add gitlab git@gitlab.com:1on1.today/1on1.git
* git push gitlab develop


## Other
* pagespeed insights
* tiny jpg
* Standard code style: php /usr/local/lib/php-code-quality/vendor/bin/phpcbf --standard=ruletest.xml .
* Laradock
https://medium.com/mr-efacani-teatime/%E5%9C%A8%E5%AF%A6%E9%9A%9B%E5%B0%88%E6%A1%88%E9%96%8B%E7%99%BC%E4%B8%8A%E4%BD%BF%E7%94%A8docker%E6%89%80%E5%B8%B6%E4%BE%86%E7%9A%84%E6%95%88%E7%9B%8A-7e6abc23181d

* sudo dpkg-reconfigure tzdata => 避免ubuntu shutdown時被MySQL卡住

## Laravel
* Create Project
1. composer create-project laravel/laravel project--name --prefer-dist
2. php artisan key:generate
3. chmod 777 -R storage/

