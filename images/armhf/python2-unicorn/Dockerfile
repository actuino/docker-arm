FROM actuino/python2-armhf-dev:1
#FROM alexellis2/python2-armhf:2

#RUN apt-get -q update && apt-get -qy install python-dev python-pip build-essential && \

RUN  pip install -I rpi_ws281x && \
  pip install unicornhat &&  \
	rm -rf /var/lib/apt/lists/* && \
	apt-get -qy clean all

ENTRYPOINT []

WORKDIR /root/
COPY rainbow.py rainbow.py
#CMD ["python2","./rainbow.py"]
CMD ["/bin/bash"]