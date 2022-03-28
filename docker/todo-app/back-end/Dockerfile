FROM node:14-alpine AS build

EXPOSE 3001

WORKDIR /app

ADD node_modules.tar.gz ./

COPY package*.json ./

RUN npm install

COPY ./ ./

ENTRYPOINT [ "npm", "start" ]