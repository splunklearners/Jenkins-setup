FROM centos
RUN yum -y install httpd
EXPOSE 80
COPY index.html /var/www/html/
WORKDIR /var/www/html
ENTRYPOINT [ "/usr/sbin/httpd" ]
CMD ["-D", "FOREGROUND"]
