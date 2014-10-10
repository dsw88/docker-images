FROM dsw88/debian7

MAINTAINER "David Woodruff <dswoodruff88@gmail.com>"

RUN apt-get update; \
    apt-get -y install \
      wget \
      git

RUN wget --quiet --no-check-certificate http://golang.org/dl/go1.3.linux-amd64.tar.gz; \
    tar -xzf go1.3.linux-amd64.tar.gz --directory /usr/local; \
    rm go1.3.linux-amd64.tar.gz

ENV PATH $PATH:/usr/local/go/bin
ENV GOPATH /go
ENV PATH $PATH:/go/bin
