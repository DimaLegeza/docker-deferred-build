FROM ubuntu:latest

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install python -y && \
    mkdir /usr/local/bin/sources

ONBUILD COPY ./sources/main.py /usr/local/bin/sources

COPY entrypoint.sh /usr/local/bin

ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
