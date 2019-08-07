#This sample docker for testapp front end
FROM centos:7
MAINTAINER vijaypatil85@gmail.com
RUN yum -y update
RUN yum -y install httpd
#COPY code/* /var/www/html
# folder content(not folder). ADD will unzip and copy if zip file, allows copy from internet (url)
ADD code /var/www/html
ENV BACKENLB=test
EXPOSE 80
COPY config/httpd-foreground /usr/bin
RUN chmod 755 /usr/bin/httpd-foreground
CMD ["httpd-foreground"]
#CMD ["apchectl", "-D" "FOREGROUND"]
#ENTRYPOINT 
#USER apache
#WORKDIR 
#VOLUME 


