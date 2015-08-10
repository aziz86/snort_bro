#The source image
FROM ubuntu:14.04

#Maintainer of Dockerfile
MAINTAINER Laaziz LAHLOU <lahlou.laaziz@gmail.com>

#Update APT and install HAProxy and Balance
RUN apt-get update --fix-missing && apt-get install -y supervisor nano wget libnet-socks-perl libnet-cidr-perl nmap
RUN apt-get update --fix-missing && apt-get install -y mgen
RUN apt-get update --fix-missing && apt-get install -y tcpreplay
#RUN apt-get update --fix-missing && apt-get install -y build-essential libgeoip-dev libpcap-dev libssl-dev python-dev zlib1g-dev php5-curl \
#git-core bison cmake flex gawk make swig curl wget g++ gcc


RUN wget http://iweb.dl.sourceforge.net/project/inundator/0.5/inundator_0.5_all.deb
RUN dpkg -i inundator_0.5_all.deb 

#RUN apt-get clean
#RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
#RUN wget https://www.bro.org/downloads/release/bro-2.4.tar.gz
#RUN tar xzf bro-2.4.tar.gz 
#RUN cd bro-2.4 && ./configure && make && make install
#ENV PATH /usr/local/bro/bin:$PATH

CMD ["/bin/bash"]
