FROM alpine:latest

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update && apk add bash

ADD ./dist/ratings-linux-amd64 app
ADD ./configs/ratings.yml .
ADD ./scripts/wait-for .


