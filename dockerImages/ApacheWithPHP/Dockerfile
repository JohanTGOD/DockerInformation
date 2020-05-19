FROM centos:7
WORKDIR /var/www/html
RUN \
  yum -y install httpd && \
  yum -y install php && \
  yum -y install php-cli && \
  yum -y install php-common
RUN echo "<?php phpinfo(); ?>" > ./hola.php
COPY html5up-massively .
CMD apachectl -DFOREGROUND
