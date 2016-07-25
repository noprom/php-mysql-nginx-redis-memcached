FROM nginx:1.9.0

ADD  nginx.conf      /etc/nginx/nginx.conf
ADD  sites-enabled/*    /etc/nginx/conf.d/
RUN  mkdir /app/www && mkdir /app/log && mkdir /app/log/nginx && mkdir /app/log/phpsession && mkdir /app/log/php
RUN  chown -R www-data.www-data /app/www /app/log

EXPOSE 80
VOLUME ["/app"]

