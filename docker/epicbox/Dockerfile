FROM ubuntu:latest
LABEL authors="@crackaf"

# Install python3, pip3, python2, pip2, g++, and nodejs lts
RUN apt-get update && apt-get install -y \
  python3 \
  python3-pip \
  g++ \
  gcc \
  make \
  curl \
  && \
  curl -sL https://deb.nodesource.com/setup_16.x | bash - && \
  apt-get install -y nodejs && \
  apt-get clean && \
  pip3 install --upgrade pip && \
  npm install -g yarn && \
  npm cache clean --force && \
  rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* /root/.cache 
