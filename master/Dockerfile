FROM ubuntu:18.04

RUN apt-get update -y && \
    apt-get install -y python3-pip python3-dev

RUN pip3 install pika

RUN pip3 install requests

RUN pip3 install docker

WORKDIR /app

ENV IS_MASTER=True

COPY . /app

ENTRYPOINT [ "python3" ]

CMD [ "app.py" ]
