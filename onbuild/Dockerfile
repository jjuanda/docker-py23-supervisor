FROM jjuanda/py23-supervisor

MAINTAINER Juan Daniel López Serna

# Onbuild hook 
RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

ONBUILD COPY requirements.txt /usr/src/app/
ONBUILD RUN pip3 install -r requirements.txt

ONBUILD COPY . /usr/src/app