FROM nginx

RUN apt-get update && apt-get upgrade -y

COPY default.conf /etc/nginx/conf.d/default.conf

VOLUME /var/log/nginx /var/log/nginx

EXPOSE 8888

CMD service nginx start && /bin/bash
