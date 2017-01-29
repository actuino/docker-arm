FROM resin/rpi-raspbian
USER root

RUN apt-get update && \
    apt-get -qy install ca-certificates python python-dev python-pip git build-essential && \
	pip install rpi.gpio && \
    rm -rf /var/lib/apt/lists/* && \
    apt-get -qy clean all && \
	alias 'll'='ls -al'
CMD ["python"]
