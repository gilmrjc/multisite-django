FROM nginx:stable-alpine

MAINTAINER Gildardo Adrian Maravilla Jacome "gilmrjc@gmail.com"

COPY master.conf /etc/nginx/conf.d/master.conf

ENTRYPOINT ["nginx", "-g", "daemon off;"]
