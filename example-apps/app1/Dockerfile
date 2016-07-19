FROM gilmrjc/multisite-django:dev-onbuild

MAINTAINER Gildardo Adrian Maravilla Jacome "gilmrjc@gmail.com"

COPY requirements.txt /requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

RUN addgroup django && \
    adduser django -G django -h /usr/src/app -D && \
    chown -R django:django /usr/src/app

USER django

RUN ["/usr/src/app/manage.py", "migrate"]
