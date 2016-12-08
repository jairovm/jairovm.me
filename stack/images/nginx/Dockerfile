FROM resin/rpi-raspbian:jessie

RUN apt-get update \
    && apt-get install -y nginx \
    && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

#COPY conf/ /etc/nginx/
#COPY ssl/ /etc/nginx/ssl

EXPOSE 80 443

CMD ["nginx", "-g", "daemon off;"]

