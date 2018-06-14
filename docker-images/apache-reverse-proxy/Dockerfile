FROM php:7.0-apache

MAINTAINER Marie Lemdjo <marie.lemdjonzinke@heig-vd.ch>   

COPY conf/ /etc/apache2 
 
RUN a2ensite 000-* 001-*
RUN a2enmod proxy proxy_http 
