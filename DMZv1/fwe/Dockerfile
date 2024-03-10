FROM alpine:latest
RUN apk update 
RUN apk add vim openssl curl tcpdump lftp ulogd
RUN apk add hping3 --update-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing
COPY ./net.ipv4.conf /etc/sysctl.d
COPY ./entrypoint.sh /
COPY ./ulogd.conf /etc/.