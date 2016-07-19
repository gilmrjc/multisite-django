FROM gilmrjc/multisite-django:dev-onbuild

MAINTAINER Gildardo Adrian Maravilla Jacome "gilmrjc@gmail.com"

COPY requirements.txt /requirements.txt

RUN pip install --no-cache-dir -r requirements.txt

RUN ["/usr/src/app/manage.py", "migrate"]
