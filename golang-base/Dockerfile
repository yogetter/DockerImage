FROM ubuntu:16.04

RUN apt-get update && apt-get install -y git wget && \
    wget https://dl.google.com/go/go1.10.2.linux-amd64.tar.gz && \
	tar -C /usr/local -xzf go1.10.2.linux-amd64.tar.gz 

ENV PATH $PATH:/usr/local/go/bin
