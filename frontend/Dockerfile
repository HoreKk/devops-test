FROM node:12-alpine as builder

WORKDIR /

COPY *.json /

RUN npm install

COPY . ./

RUN npm run build