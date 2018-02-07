FROM httpd 
RUN groupadd www && useradd -g www -s /sbin/nologin www
VOLUME /var/www/ 
VOLUME /usr/local/apache2/logs
COPY httpd.conf /usr/local/apache2/conf/httpd.conf
COPY httpd-vhost.conf /usr/local/apache2/conf/extra/httpd-vhosts.conf
