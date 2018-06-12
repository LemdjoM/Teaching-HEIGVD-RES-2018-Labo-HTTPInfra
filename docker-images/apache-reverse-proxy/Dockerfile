FROM php:5.6-apache

MAINTAINER Marie Lemdjo <marie.lemdjonzinke@heig-vd.ch> 

RUN apt-get update && \
	apt-get install -y nano

COPY apache2-foreground /user/local/bin/
COPY template /var/apache2/templates	

COPY conf/ /etc/apache2 
 
RUN a2ensite 000-* 001-*
RUN a2enmod proxy proxy_http 
