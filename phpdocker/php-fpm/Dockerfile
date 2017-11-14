FROM phpdockerio/php7-fpm:latest
WORKDIR "/application"

# Install selected extensions and other stuff
RUN apt-get update \
    && apt-get -y --no-install-recommends install  php7.0-memcached php7.0-mysql php7.0-redis php7.0-sqlite3 php7.0-gd php7.0-imagick php7.0-soap \
    && apt-get clean; rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /usr/share/doc/*