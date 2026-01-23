FROM node:22-alpine

WORKDIR /opt

COPY . .

RUN npm install && npm run build

RUN apk add apache2

RUN cp dist/* /var/www/localhost/htdocs/

EXPOSE 80

CMD ["httpd", "-D", "FOREGROUND"]
