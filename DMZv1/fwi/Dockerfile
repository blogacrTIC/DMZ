FROM alpine:latest
RUN apk update 
RUN apk add vim openssl curl lftp
COPY ./net.ipv4.conf /etc/sysctl.d
COPY ./entrypoint.sh /