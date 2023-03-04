FROM python:slim-buster

RUN python3 -m venv /opt/venv && \
    . /opt/venv/bin/activate && \
    pip install --upgrade pip &&\
    pip install flask redis && \
    groupadd -r flask && useradd -r -g flask flask && \
    mkdir /src && \
    chown -R flask:flask /src

USER flask

ADD app.py /src/app.py

WORKDIR /src

ENV FLASK_APP=app.py REDIS_HOST=redis

EXPOSE 5000

CMD ["flask", "run", "-h", "0.0.0.0"]