#VERSION 0.0.1
#symfony3 基于apache2 php5实现
FROM mobingi/ubuntu-apache2-php5
#签名
MAINTAINER xcyxiner "xcyxiner@me.com"
RUN LC_ALL=C.UTF-8  add-apt-repository -y ppa:ondrej/php
RUN apt-get update
#symfony 初始化必须
RUN apt-get install -y  php5.6-xml
#mongodb php
RUN apt-get install -y  php-mongodb
#amqp php
RUN apt-get install -y php5.6-mbstring
RUN apt-get install -y php5.6-bcmath
#dev操作
#git 
RUN apt-get install -y git
#vim中文乱码
ADD .vimrc  /root/.vimrc
#默认目录
WORKDIR /var/www/html
#bash 无法输入中文
ENV LANG C.UTF-8
#安装 tree
RUN apt-get install -y tree
#时区
ADD usr_share_zoneinfo_Asia_Shanghai /etc/localtime
#vim
RUN apt-get install -y vim
#Composer
RUN apt-get install -y curl
RUN apt-get install -y  zip unzip
RUN curl -sS https://getcomposer.org/installer | php
RUN mv composer.phar /usr/local/bin/composer
#phpunit
RUN apt-get install -y wget
RUN  wget -O phpunit https://phar.phpunit.de/phpunit-5.phar
RUN chmod +x phpunit
RUN mv  phpunit /usr/local/bin/phpunit
#update apache config
ADD 000-default.conf /etc/apache2/sites-available/000-default.conf
#w3m
RUN apt-get install -y w3m
#ext-mongo ^1.5
RUN apt-get install php-mongo
