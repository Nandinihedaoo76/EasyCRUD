FROM node:22-alpine

WORKDIR /opt

COPY . .

RUN npm install

EXPOSE 80

ENTRYPOINT [ "npm", "start" ]

