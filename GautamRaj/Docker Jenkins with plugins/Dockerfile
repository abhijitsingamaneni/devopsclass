# using jenkins image
# Build image with:  docker build -t axndj1993/jenkins:1.05 .

FROM jenkins/jenkins
MAINTAINER Gautam Raj
ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
COPY plugins.txt /usr/share/jenkins/ref/plugins.txt
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
