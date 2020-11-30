FROM debian:10.6-slim 

ARG awscliVersion=2.0.30

RUN apt-get update && apt-get upgrade -y && apt-get install -y curl unzip 
RUN curl https://awscli.amazonaws.com/awscli-exe-linux-x86_64-${awscliVersion}.zip -o awscliv2.zip
RUN unzip awscliv2.zip
RUN ./aws/install -i /usr/local/aws-cli -b /usr/local/bin

ENTRYPOINT ["/usr/local/bin/aws"]
