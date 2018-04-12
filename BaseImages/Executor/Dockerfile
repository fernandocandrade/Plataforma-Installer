FROM python:3.6.3-slim

WORKDIR /deps

RUN apt-get update -y && apt-get install git -y && apt-get install wget -y

RUN wget https://raw.githubusercontent.com/ONSBR/Plataforma-Executor/master/requirements.txt

RUN pip install -U pip gunicorn
RUN pip install -r requirements.txt