FROM node:12-alpine as builder

WORKDIR /

COPY *.json /

RUN npm install

COPY . ./

RUN npm run build

FROM nginx

COPY --from=builder /build /usr/share/nginx/html

ENV NGINX_PORT=80