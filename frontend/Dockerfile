FROM node:15.14-alpine

WORKDIR /app

EXPOSE 3000

COPY package.json package-lock.json ./

RUN npm i --silent

COPY . ./

CMD [ "npm", "start" ]