# Sử dụng image MySQL chính thức
FROM mysql:5.7

# Thiết lập các biến môi trường cho MySQL
ENV MYSQL_ROOT_PASSWORD=rootpassword
ENV MYSQL_DATABASE=phpdb
ENV MYSQL_USER=phpuser
ENV MYSQL_PASSWORD=phppassword

# Copy tệp .sql để khởi tạo database
COPY post.sql /docker-entrypoint-initdb.d/

# Expose cổng 3306 cho MySQL
EXPOSE 3306

CMD ["mysqld"]
