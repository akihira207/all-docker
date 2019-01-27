FROM nginx:1.13.9-alpine

RUN apk --update --no-cache add tzdata && \
    cp /usr/share/zoneinfo/Asia/Tokyo /etc/localtime && \
    apk del tzdata

RUN apk add --update coreutils openssh-client && rm -rf /var/cache/apk/*

ADD nginx.conf /etc/nginx/nginx.conf
