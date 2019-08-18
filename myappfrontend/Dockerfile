#Dockerfile from myapp front end runs on apache
FROM centos:7
MAINTAINER khalindar@gmail.com
RUN yum -y update
RUN yum -y install httpd
ADD code /var/www/html
#COPY code/* /var/www/html
EXPOSE 80
#RUN useradd mysvcuser
#USER mysvcuser
WORKDIR /apps
ADD config /opt
RUN chmod 755 /opt/myenv
RUN /opt/myenv
#USER root
ENV BACKENDLB=test
#RUN yum -y update ----> sh -c yum -y update
CMD ["httpd", "-D", "FOREGROUND"]
#CMD 




ENTRYPOINT 

