FROM debian:9-slim

RUN apt-get update && apt-get install -y python3-pip groff
RUN pip3 install awscli --upgrade --user

# Add aws and other pip-installed dependencies to PATH
ENV PATH "${PATH}:/root/.local/bin"

VOLUME "/data"

ENTRYPOINT ["/root/.local/bin/aws"]
