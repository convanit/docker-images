FROM quay.io/quarkus/centos-quarkus-maven:21.0.0-java11
USER root
RUN yum install -y gcc-c++ make
RUN curl -sL https://rpm.nodesource.com/setup_15.x | bash -
RUN yum install -y nodejs
RUN npm install --global yarn
RUN yum install -y zip unzip
USER quarkus
CMD [ "node --version" ]

## docker build -t centos-quarkus-maven-node:21.0.0-java11-node15 .
## docker run -it docker.io/library/centos-quarkus-maven-node:21.0.0-java11-node15 yarn --version 