FROM node:18.20.0-alpine3.19
EXPOSE 8080
# Create a group and user
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop
WORKDIR /opt/server
RUN chown roboshop:roboshop /opt/server/
USER roboshop
RUN apt-get remove -y sudo && \
    usermod -p '!' root
ENV MONGO=true
COPY package.json /opt/server/
RUN npm install
COPY server.js /opt/server/
CMD ["node","server.js"]
