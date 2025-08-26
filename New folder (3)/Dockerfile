# Use official PHP with Apache
FROM php:8.2-apache

# Enable common PHP extensions (like MySQL if needed)
RUN docker-php-ext-install mysqli && docker-php-ext-enable mysqli

# Copy your project into the Apache web directory
COPY . /var/www/html/

# Give proper permissions
RUN chown -R www-data:www-data /var/www/html \
    && chmod -R 755 /var/www/html

# Expose web server port
EXPOSE 80
