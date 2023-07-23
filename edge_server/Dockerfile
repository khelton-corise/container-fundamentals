# using apache httpd base image
FROM nginx:stable-alpine3.17-slim

# labels for the image
LABEL org.opencontainers.image.authors="khelton2003@gmail.com"
LABEL org.opencontainers.image.server_type="edge_server"
LABEL org.opencontainers.image.source=https://github.com/khelton-corise/container-fundamentals
LABEL org.opencontainers.image.description="Containter Fundamentals - Static Website Image"
LABEL org.opencontainers.image.licenses=APACHE2

# copy the files over apache server directory
COPY config/nginx.conf /etc/nginx/
COPY web_content/ /var/www
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]