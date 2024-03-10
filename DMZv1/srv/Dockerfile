FROM alpine:latest
RUN adduser -h /home/usr -s /bin/ash  -D -u 1000 usr
RUN echo 'usr:12345' | chpasswd
RUN apk update 
RUN apk add openrc
RUN apk add vim openssl curl php lftp pure-ftpd
RUN apk add hping3 --update-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing
COPY ./entrypoint.sh /