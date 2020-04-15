FROM ubuntu:16.04

MAINTAINER Alida "305930@supinfo.com"
WORKDIR /app
RUN apt-get update -y && \
    apt-get install -y python-pip python-dev

COPY ./requirements.txt /app/requirements.txt

RUN pip install -r requirements.txt

COPY . /app

ENTRYPOINT [ "python" ]
CMD [ "student_age.py" ]
