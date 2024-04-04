FROM node:18.20.0-alpine3.19

EXPOSE 8080

ENV MONGO=true

WORKDIR /opt/server

COPY package.json /opt/server/

RUN npm install

COPY server.js /opt/server/

CMD ["node","server.js"]
