# Sử dụng PHP với Apache
FROM php:7.4-apache

# Copy mã nguồn PHP vào container
COPY . /var/www/html/

# Cài đặt các extension cần thiết cho PHP
RUN docker-php-ext-install mysqli \
    && chown -R www-data:www-data /var/www/html

# Expose cổng 80 cho các router
EXPOSE 80

CMD ["apache2-foreground"]
