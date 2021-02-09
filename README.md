## What is this?
This is the official Wordpress with PHP 7.4 **FPM** base image with additional `redis` and other extensions. There are modifications to the `/usr/local/etc/php-fpm.d/zz-docker.conf` file which forces PHP to listen on a UNIX socket at `/sock/docker.sock`. It would require a web server such as NGINX to send requests upstream to this same UNIX socket in order to work.

## What's included:
* PHP extensions (additional to default PHP installation):
  * `redis`
  * `imagick`
  * `libsodium`
  * `exif`
  * `gettext`
  * `intl`
  * `mcrypt`
  * `socket`
  * `zip`

## TODO:
- [x] Add `redis` PHP extensions and others required for Wordpress
