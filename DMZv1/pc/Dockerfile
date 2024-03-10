FROM alpine:latest
RUN apk update 
RUN apk add vim openssl curl php lftp
RUN apk add hping3 --update-cache --repository http://dl-cdn.alpinelinux.org/alpine/edge/testing
COPY ./entrypoint.sh /