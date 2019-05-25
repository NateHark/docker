FROM debian:9-slim

ARG hugoVersion

RUN apt-get update && apt-get install -y \
      wget

RUN wget --quiet -O /tmp/hugo.tar.gz \
        https://github.com/gohugoio/hugo/releases/download/v${hugoVersion}/hugo_extended_${hugoVersion}_Linux-64bit.tar.gz && \
    tar -zxf /tmp/hugo.tar.gz -C /tmp && \
    cp /tmp/hugo /usr/bin/hugo
