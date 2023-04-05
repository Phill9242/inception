# Penultimate Alpine Version
FROM alpine:3.16

# Att and install of nginx
RUN apk update && apk upgrade && apk add nginx

#  NGINX folder
RUN mkdir -p /run/nginx

# nginx config
COPY ./conf/nginx.conf /etc/nginx/nginx.conf

# PORT exposure
EXPOSE 443

# NGINX start
CMD ["nginx", "-g", "daemon off;"]
