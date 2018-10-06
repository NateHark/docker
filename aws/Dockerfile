FROM alpine:latest

RUN apk update && apk add python py-pip groff
RUN pip install awscli --upgrade --user

# Add aws and other pip-installed dependencies to PATH
ENV PATH "${PATH}:/root/.local/bin"

VOLUME "/data"

ENTRYPOINT ["/root/.local/bin/aws"]
