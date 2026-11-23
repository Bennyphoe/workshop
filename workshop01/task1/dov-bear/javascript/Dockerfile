FROM node:26-bookworm

ARG APP_DIR=/app

WORKDIR ${APP_DIR}

COPY main.js .
COPY package.json .
COPY public public
COPY views views

RUN npm install

ENV PORT=3000
ENV INSTANCE_NAME=""
ENV INSTANCE_HASH=""

ENTRYPOINT node main.js