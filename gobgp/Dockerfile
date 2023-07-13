FROM golang:latest

WORKDIR /go/src

RUN git clone https://github.com/osrg/gobgp.git \
    && cd gobgp \
    && go install ./cmd/gobgpd \
    && go install ./cmd/gobgp

RUN apt-get update && apt-get install -y iputils-ping telnet

RUN mkdir /root/gobgp
VOLUME [ "/root/gobgp" ]
