FROM python:3.9-slim-buster

RUN apt-get update && \
    apt-get -y install gcc default-libmysqlclient-dev

WORKDIR /api

COPY ./api /api

COPY ./docker/flask/requirements.txt /api 
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

CMD ["flask", "run"]