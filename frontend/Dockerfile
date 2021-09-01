FROM node:12-alpine as builder

WORKDIR /

COPY *.json /

RUN npm install

COPY src ./src
COPY public ./public

RUN npm run build