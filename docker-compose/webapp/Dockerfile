FROM tecadmin/ubuntu-ssh:16.04

RUN apt-get update \
&amp;&amp; apt-get install -y apache2

COPY index.html /var/www/html/
WORKDIR /var/www/html
CMD [&quot;apachectl&quot;, &quot;-D&quot;, &quot;FOREGROUND&quot;]
EXPOSE 80
