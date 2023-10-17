FROM node:18.18.2-alpine

RUN apk update && \
  apk add --no-cache bash

RUN npm i -g @nestjs/cli

RUN npm i -g pnpm

WORKDIR /app

COPY package.json pnpm-lock.yaml ./

RUN pnpm i
