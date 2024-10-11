FROM alpine:3.11.10 as frontendbuilder

RUN mkdir /frontend
WORKDIR /frontend

RUN apk add --no-cache npm

COPY package.json .
RUN npm install

COPY ./ ./

RUN npm run build