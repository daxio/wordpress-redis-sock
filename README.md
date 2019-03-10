## What is this?
This is the official Wordpress with PHP 7.3 **FPM** base image with additional `redis` and other extensions. There's one `sed` line meant to delete the line in `/usr/local/etc/php-fpm.d/zz-docker.conf` which forces PHP to listen on a TCP port. It would require a web server such as NGINX to send requests upstream to a UNIX socket in order to work.

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
