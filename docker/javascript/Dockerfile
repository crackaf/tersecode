FROM node:lts-alpine
LABEL authors="@crackaf"
RUN adduser -DH -h /sandbox sandbox

RUN mkdir /sandbox
WORKDIR /sandbox

RUN npm install \
  synchro-prompt
