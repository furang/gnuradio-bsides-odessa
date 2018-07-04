FROM ubuntu:xenial

RUN apt-get update
RUN apt-get install -y \
    apt-transport-https \
    ca-certificates \
    curl \
    software-properties-common

RUN add-apt-repository ppa:opencpn/opencpn
RUN apt-get update
RUN apt-get install -y opencpn

EXPOSE 10110/udp

CMD opencpn
