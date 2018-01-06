# docker_symfony
symfony docker container

# reference
* [The requested PHP extension dom is missing from your system](https://stackoverflow.com/questions/44952650/the-requested-php-extension-dom-is-missing-from-your-system/44963112)
* [how-to-install-mongodb-php-extension-in-ubuntu-16-04-lts](https://askubuntu.com/questions/765146/how-to-install-mongodb-php-extension-in-ubuntu-16-04-lts)
* [php-amqplib/php-amqplib](https://packagist.org/packages/php-amqplib/php-amqplib)

# how to  use
https://hub.docker.com/r/nimmis/apache-php7/

# eg

```
docker run  -d  -p 8080:80  -v /path/to/websource:/var/www/html  xcyxiner/symfony
```
