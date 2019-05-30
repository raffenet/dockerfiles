FROM centos:7
MAINTAINER Ken Raffenetti raffenet@mcs.anl.gov
RUN yum install -y \
    wget \
    tar \
    gzip \
    perl \
    perl-Data-Dumper \
    which \
    patch \
    m4 \
    gcc \
    gcc-c++ \
    gcc-gfortran \
    make

RUN cd /tmp && wget http://mirror.team-cymru.com/gnu/autoconf/autoconf-2.69.tar.gz && tar xfz autoconf-2.69.tar.gz && cd autoconf-2.69 && ./configure && make install

RUN cd /tmp && wget http://mirror.team-cymru.com/gnu/automake/automake-1.16.1.tar.gz && tar xfz automake-1.16.1.tar.gz && cd automake-1.16.1 && ./configure && make install

RUN cd /tmp && wget http://mirror.team-cymru.com/gnu/libtool/libtool-2.4.6.tar.gz && tar xfz libtool-2.4.6.tar.gz && cd libtool-2.4.6 && ./configure && make install
