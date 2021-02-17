FROM ubuntu:latest

LABEL MANTAINER="Francesco Cataldo"

USER root

RUN apt-get update && apt-get install -y redis-server

EXPOSE 6380/tcp

USER redis

COPY ./redis.conf /etc/redis/redis.conf

ENTRYPOINT ["redis-server", "/etc/redis/redis.conf"]

