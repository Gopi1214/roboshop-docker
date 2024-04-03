FROM nginx

RUN rm -rf /usr/share/nginx/html/index.html

RUN rm -rf /etc/nginx/nginx.conf

RUN rm -rf /etc/nginx/conf.d/default.conf

RUN rm -rf /etc/nginx/default.d/roboshop.conf

COPY roboshop.conf /etc/nginx/default.d/

ADD static /usr/share/nginx/html/


