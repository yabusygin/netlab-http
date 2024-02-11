FROM nginx:1.25.3

RUN mkdir /srv/www/

COPY default.conf /etc/nginx/conf.d/
COPY htpasswd /etc/nginx/
COPY static/ /srv/www/
