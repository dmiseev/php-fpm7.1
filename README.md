## PHP-FPM Image

[![Build Status](https://travis-ci.com/dmiseev/php-fpm7.1.svg?branch=master)](https://travis-ci.com/dmiseev/php-fpm7.1)

 **Helpful PHP-FPM image from official ubuntu:xenial**
 
 >
 > PHP-FPM version - 7.1.33
 >
 > DateTime - Europe/Kiev
 >
 > Supervisor installed globally
 >
 > Composer installed globally

## Tags
 * dmiseev/php-fpm7.1:stable

### Extensions:

 * php7.1-pgsql
 * php7.1-mysql
 * php7.1-opcache
 * php7.1-common
 * php7.1-mbstring
 * php7.1-mcrypt
 * php7.1-soap
 * php7.1-cli
 * php7.1-intl
 * php7.1-json
 * php7.1-xsl
 * php7.1-imap
 * php7.1-ldap
 * php7.1-curl
 * php7.1-gd
 * php7.1-dev
 * php7.1-fpm
 * php7.1-redis
 * php7.1-memcached
 * php7.1-mongodb
 * php7.1-bcmath
 * php7.1-imagick (`new`)
 * php7.1-zip (`new`)
 * php7.1-zmq (`new`)
 * php7.1-apcu (`new`)

### In addition

 * Supervisor (installed globally)
 * Composer (installed globally)
 
### Docker Compose yml

```yaml
version: "2"
services:
 php-fpm:
   image: dmiseev/php-fpm7.1
   volumes:
    - .:/usr/local/src/app
   working_dir: /usr/local/src/app
   extra_hosts:
    - "app:127.0.0.1"
```
