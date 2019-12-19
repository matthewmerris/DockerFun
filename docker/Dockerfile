FROM ubuntu:18.04
MAINTAINER Matthew Merris

# A simple demo of installing the LAPACKE library with a demo c application
# to ensure proper inclusion of the library

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y gcc
RUN apt update 
RUN apt-get install -y liblapack3 
RUN apt-get install -y liblapack-dev 
RUN apt-get install -y libopenblas-base 
RUN apt-get install -y libopenblas-dev 
RUN apt-get install -y liblapacke-dev 
RUN apt-get install -y liblapack-dev
RUN apt-get install -y git
RUN git clone https://github.com/vT3k/DockerFun.git
RUN gcc ./DockerFun/callingDGELS.c -o callingDGELS -llapacke && ./callingDGELS
