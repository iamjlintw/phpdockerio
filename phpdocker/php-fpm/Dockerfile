FROM phpdockerio/php7-fpm:latest

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php7.0-memcached php7.0-mongodb php7.0-mysql php7.0-pgsql php7.0-redis php7.0-sqlite3 php7.0-gd php7.0-geoip php7.0-imagick php7.0-imap php7.0-mbstring php7.0-msgpack php7.0-phpdbg php7.0-ssh2 php7.0-xdebug php7.0-xmlrpc php7.0-xsl \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*


WORKDIR "/application"