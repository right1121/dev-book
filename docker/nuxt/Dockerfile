FROM node:14.15.4-alpine

EXPOSE 3000
ENV HOST 0.0.0.0


WORKDIR /app
COPY ./nuxt /api
COPY ./docker/nuxt/dev-init.sh /api

RUN apk update
RUN yarn install
