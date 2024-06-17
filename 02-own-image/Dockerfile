FROM        docker.io/redhat/ubi9
RUN         dnf install nginx -y
RUN         rm -rf /usr/share/nginx/html/*
ADD         index.html /usr/share/nginx/html
ENTRYPOINT  ["nginx", "-g", "daemon off;"]


