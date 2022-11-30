FROM 314682408916.dkr.ecr.us-east-1.amazonaws.com/task-21:nginx-alpine

RUN apk update && apk upgrade && \
    apk add --no-cache --upgrade bash && \
    mkdir /usr/share/nginx/html/static/
COPY trainee.conf /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/nginx.conf
WORKDIR /usr/share/nginx/html/static/
COPY static/ .

EXPOSE 80


