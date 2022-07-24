FROM scratch
ADD ubuntu-focal-oci-amd64-root.tar.gz /
CMD ["bash"]

RUN sudo apt update
RUN apt install apache2
RUN systemctl start apache2

# Copy apache vhost file to proxy php requests to php-fpm container
COPY demo.apache.conf /usr/local/apache2/conf/demo.apache.conf
RUN echo "Include /usr/local/apache2/conf/demo.apache.conf" \
    >> /usr/local/apache2/conf/httpd.conf
