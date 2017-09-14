FROM golang:1.9-alpine3.6

RUN apk add --no-cache make bash git librdkafka-dev g++ glide && \
    mkdir /lib64 && ln -s /lib/libc.musl-x86_64.so.1 /lib64/ld-linux-x86-64.so.2 &&\
    go get -u -v github.com/alecthomas/gometalinter && \
    gometalinter --install
