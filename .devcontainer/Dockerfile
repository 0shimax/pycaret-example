FROM python:3.8-slim-buster

RUN apt-get update \
    && apt-get install -y --no-install-recommends \
    curl wget gosu jq unzip libgomp1 default-libmysqlclient-dev python3-dev

COPY requirements.txt /tmp/
RUN pip install --upgrade pip && \
    pip install -r /tmp/requirements.txt
