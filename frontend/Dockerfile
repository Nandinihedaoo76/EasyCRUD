FROM node:22-alpine

WORKDIR /opt

COPY . .

RUN npm install && npm run build

RUN apk add apache2

COPY dist/ /var/www/localhost/htdocs/

EXPOSE 3000

CMD ["httpd", "-D", "FOREGROUND"]
