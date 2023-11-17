FROM alpine
COPY ssh_config /etc/ssh/ssh_config
RUN sed -i "s/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g" /etc/apk/repositories \
    && apk add --no-cache openssl-dev openssh-client sshpass curl zip unzip && rm -rf /var/cache/apk/*
