FROM ubuntu:20.04
ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
apt-get install -y apache2 && \
apt-get clean


ENV APACHE_LOG_DIR /var/log/apache2


ENTRYPOINT ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
