# Database Dockerfile sử dụng MySQL 5.7
FROM mysql:5.7

# Thiết lập biến môi trường cho MySQL
ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=projectdb

# Copy file SQL vào thư mục init để tự động tạo database khi container khởi chạy
COPY ./post.sql /docker-entrypoint-initdb.d/

# Mở cổng 3306 để MySQL có thể truy cập từ bên ngoài
EXPOSE 3306
