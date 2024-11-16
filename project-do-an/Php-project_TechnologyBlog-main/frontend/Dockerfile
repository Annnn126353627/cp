# Sử dụng nginx để phục vụ các file tĩnh
FROM nginx:alpine

# Copy các file tĩnh vào Nginx
COPY css/ /usr/share/nginx/html/css/
COPY js/ /usr/share/nginx/html/js/
COPY images/ /usr/share/nginx/html/images/

# Expose cổng 80 để truy cập
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
