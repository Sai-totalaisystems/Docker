FROM ubuntu:20.04
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update
RUN apt-get install -y apache2

CMD ["/usr/sbin/apache2","-D","FOREGROUND"]
EXPOSE 80
