FROM ubuntu:latest
RUN apt update -y
RUN apt install vim openssl curl -y
COPY ./net.ipv4.conf /etc/sysctl.d
COPY ./entrypoint.sh /