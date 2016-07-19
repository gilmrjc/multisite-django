FROM python:2-alpine

MAINTAINER Gildardo Adrian Maravilla Jacome

ENV DJANGO_VERSION 1.9.0

RUN pip install django~="$DJANGO_VERSION"

ONBUILD COPY . /usr/src/app

ENTRYPOINT ["/usr/src/app/manage.py", "runserver"]
