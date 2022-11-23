FROM nginx:alpine

RUN apk update && apk upgrade && \
    apk add --no-cache --upgrade bash && \
    mkdir /usr/share/nginx/html/static/
COPY trainee.conf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /usr/share/nginx/html/static/
COPY static/ .

EXPOSE 80


