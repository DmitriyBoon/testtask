FROM nginx

RUN apt-get update && apt-get upgrade -y
RUN apt-get install php-fpm -y

RUN usermod -aG www-data nginx

COPY default.conf /etc/nginx/conf.d/default.conf
COPY index.php /usr/share/nginx/html/index.php

VOLUME /var/log/nginx /var/log/nginx

CMD service nginx start && service php7.3-fpm start && /bin/bash
