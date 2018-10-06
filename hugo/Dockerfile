FROM alpine:latest

ARG hugoVersion=0.49

RUN wget --quiet -O /tmp/hugo.tar.gz \
        https://github.com/gohugoio/hugo/releases/download/v${hugoVersion}/hugo_${hugoVersion}_Linux-64bit.tar.gz && \
    tar -zxf /tmp/hugo.tar.gz -C /tmp && \
    cp /tmp/hugo /usr/bin/hugo

RUN touch /var/log/hugo.log