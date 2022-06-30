FROM ubuntu:20.04



RUN apt update && \
DEBIAN_FRONTEND=noninteractive apt install -y libapache2-mod-php7.4 php7.4-gd php7.4-curl php7.4-xml php7.4-mysqli php7.4-zip php7.4-pdo && \
apt autoclean && \
rm -rf /var/www/html/*

COPY ./shopxo/ /var/www/html
RUN chmod 777 /var/www/html -R

ENTRYPOINT /bin/bash -c 'service apache2 start; sleep 100000000;'
