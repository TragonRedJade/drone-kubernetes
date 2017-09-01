FROM nginx

ENV TERM xterm-color

RUN apt-get update \
  && apt-get install -y nano curl

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./sites-available/ /etc/nginx/sites-available

WORKDIR ["/usr/share/nginx/html"]