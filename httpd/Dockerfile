FROM httpd:alpine

RUN mkdir -p /var/run/apache2/

COPY ./httpd.conf /usr/local/apache2/conf/httpd.conf
COPY ./vhosts /usr/local/apache2/vhosts