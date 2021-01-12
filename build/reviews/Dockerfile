FROM alpine:latest

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update && apk add bash

ADD ./dist/reviews-linux-amd64 app
ADD ./configs/reviews.yml .
ADD ./scripts/wait-for .
