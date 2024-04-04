FROM ubuntu:latest as base




RUN apt-get update
RUN export DEBIAN_FRONTEND=noninteractive
RUN apt-get -y install build-essential procps curl file git


COPY installBrew.sh /installBrew.sh
RUN chmod +x /installBrew.sh
RUN /installBrew.sh

RUN brew install act
# 