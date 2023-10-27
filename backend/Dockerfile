# syntax=docker/dockerfile:1

FROM node:15-alpine

WORKDIR /app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

# Change
CMD sh -c "npm run generate && npm run migrate && node app.js"
