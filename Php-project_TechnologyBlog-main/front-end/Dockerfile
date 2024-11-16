# Front-end Dockerfile
FROM php:8.0-apache

# Copy tất cả các file từ thư mục front-end vào thư mục web của Apache
COPY ./ /var/www/html/

# Tạo các thư mục cần thiết và phân quyền
RUN chown -R www-data:www-data /var/www/html

# Mở cổng 80 để ứng dụng có thể truy cập từ bên ngoài
EXPOSE 80

# Khởi chạy Apache khi container được chạy
CMD ["apache2-foreground"]
