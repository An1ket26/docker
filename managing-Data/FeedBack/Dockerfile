FROM node:18-alpine

WORKDIR /app

COPY ["package.json","package-lock.json","/app/"]

RUN npm install

COPY . /app/

ARG DEFAULT_PORT=80

ENV PORT $DEFAULT_PORT

EXPOSE $PORT



CMD ["npm","start"]