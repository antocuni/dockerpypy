FROM i386/ubuntu:16.04
MAINTAINER Antonio Cuni <anto.cuni@gmail.com>

RUN apt-get update
RUN apt-get install -y gcc make libffi-dev pkg-config zlib1g-dev libbz2-dev \
    libsqlite3-dev libncurses5-dev libexpat1-dev libssl-dev libgdbm-dev \
    tk-dev libgc-dev python-cffi pypy mercurial

RUN apt-get install -y python-pip

RUN pip install pdbpp
COPY startup.py /root/
ENV PYTHONSTARTUP=/root/startup.py

RUN mkdir /home/antocuni
WORKDIR /home/antocuni
