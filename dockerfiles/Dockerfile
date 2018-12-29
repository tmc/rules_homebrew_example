FROM ubuntu:bionic

RUN apt-get update # Last Modified: 2018-12-28
RUN apt-get install -y build-essential
RUN apt-get install -y curl unzip git
RUN apt-get install -y sudo

ENV PATH=/home/user/bin/:$PATH
ENV LANG='en_US.UTF-8' LANGUAGE='en_US:en' LC_ALL='en_US.UTF-8'

RUN apt-get install -y locales
RUN locale-gen en_US.UTF-8

RUN groupadd -r user && useradd --no-log-init -m -g user user && adduser user sudo && echo '%sudo ALL=(ALL) NOPASSWD:ALL' >> /etc/sudoers
USER user

WORKDIR /app
