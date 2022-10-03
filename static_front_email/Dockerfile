FROM php:7.4-apache
# Install msmtp
RUN apt-get update && apt-get install msmtp msmtp-mta -y && \
rm -rf /var/lib/apt/lists/*
COPY msmtprc /etc/msmtprc
RUN chown root:msmtp /etc/msmtprc
RUN chmod 640 /etc/msmtprc
RUN echo 'sendmail_path = /usr/bin/msmtp -t' > /usr/local/etc/php/php.ini
RUN docker-php-ext-install pdo_mysql

# fichier pour le serveur de mail