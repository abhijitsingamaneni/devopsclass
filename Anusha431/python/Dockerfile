FROM python:3
MAINTAINER anusha
RUN apt-get update
RUN apt upgrade -y
WORKDIR /usr/src/app
COPY . .
CMD ["test.py"]
ENTRYPOINT ["python3"]
