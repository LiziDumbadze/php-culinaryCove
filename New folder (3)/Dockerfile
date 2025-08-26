# Use official PHP with Apache
FROM php:8.2-apache

# Copy all your project files into the Apache web root
COPY . /var/www/html/

# Give proper permissions
RUN chown -R www-data:www-data /var/www/html \
    && chmod -R 755 /var/www/html

# Expose port 80 for web traffic
EXPOSE 80

