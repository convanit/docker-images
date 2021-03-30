FROM quay.io/quarkus/centos-quarkus-maven:21.0.0-java11
USER root
RUN yum install -y gcc-c++ make
RUN curl -sL https://rpm.nodesource.com/setup_15.x | bash -
RUN yum install -y nodejs
RUN npm install --global yarn
USER quarkus
CMD [ "node --version" ]