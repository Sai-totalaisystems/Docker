FROM ubuntu:20.04
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y apache2
RUN apt-get install –y apache2-utils 
RUN apt-get clean 

ENV APACHE_RUN_DIR /var/run/apache2
CMD [“apache2”, “-D”, “FOREGROUND”]
EXPOSE 80 
