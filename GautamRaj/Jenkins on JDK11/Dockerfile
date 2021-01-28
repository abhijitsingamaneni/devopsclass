# Debain with jdk11 installed.
# Build image with:  docker build -t axndj1993/jenkins:1.04 .

FROM adoptopenjdk/openjdk11:debian-jre
MAINTAINER Gautam Raj
USER root
RUN apt-get update && apt-get install -y \
git \
vim \
sudo \
wget \
gnupg \
gnupg1 \
gnupg2 

# install jenkins
RUN wget -q -O - https://pkg.jenkins.io/debian/jenkins.io.key | sudo apt-key add -
RUN sudo sh -c 'echo deb https://pkg.jenkins.io/debian binary/ > \
    /etc/apt/sources.list.d/jenkins.list'
RUN sudo apt-get update
RUN sudo apt-get install jenkins -y

