From ubuntu:20.04

MAINTAINER faizanbashir <faizan.ibn.bashir@gmail.com>

# disable interactive functions
ENV DEBIAN_FRONTEND noninteractive

COPY sources.list /etc/apt/sources.list

RUN apt-get update

RUN apt-get install -y g++ cmake make gcc curl vim git 

RUN curl https://sh.rustup.rs -sSf | sh -s -- -y

ENV PATH="/root/.cargo/bin:${PATH}"

COPY cargo_config /root/.cargo/config


CMD ["/bin/bash"]
