FROM nginx

RUN rm -rf /usr/share/nginx/html/index.html

RUN rm -rf /etc/nginx/default.d/

COPY roboshop.conf /etc/nginx/default.d/roboshop.conf

ADD static /usr/share/nginx/html/


