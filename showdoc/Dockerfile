FROM php:5.6-apache
# COPY ./ /var/www/html/
COPY sources.list /etc/sources.list
# COPY apache2.conf /etc/apache2/apache2.conf

RUN  \
	# sed -i  's#http[:]//deb[^/ ]\+#http://ftp.cn.debian.org#g' /etc/apt/sources.list  && \
     	apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libmcrypt-dev \
        libpng-dev \
	# libapache2-mpm-itk \
    && docker-php-ext-install -j$(nproc) gd mcrypt zip


RUN \
	mkdir /var/www/html/showdoc && chmod -R 777 /var/www/html/

CMD ["apache2-foreground"]
