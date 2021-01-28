FROM ubuntu:latest
MAINTAINER rupa
RUN apt-get update
RUN apt upgrade -y
WORKDIR /
RUN mkdir /cicd
WORKDIR /cicd
RUN echo "Hello World" >> test.txt
RUN apt-get install vim -y
