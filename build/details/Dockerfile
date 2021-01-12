FROM alpine:latest

RUN sed -i 's/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update && apk add bash

ADD ./dist/details-linux-amd64 app
ADD ./configs/details.yml .
ADD ./scripts/wait-for .


