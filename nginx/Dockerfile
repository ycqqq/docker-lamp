FROM nginx
RUN groupadd www && useradd -g www -s /sbin/nologin www
VOLUME /var/www/html
COPY ./conf/nginx.conf /etc/nginx/nginx.conf
COPY ./conf/conf.d/ /etc/nginx/conf.d