FROM ubuntu:18.04

# Install dependencies
RUN apt-get update
RUN apt-get -y install apache2
RUN apt-get -y install python3 python3-pip

COPY . /python
WORKDIR /python

# RUN sudo apt-get install python3
RUN pip3 install -r requirements.txt
CMD python3 --version