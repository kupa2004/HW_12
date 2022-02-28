FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install -y \
default-jdk \
 maven \
 git \
WORKDIR /home
RUN git clone https://github.com/kupa2004/App42.git
WORKDIR /home/App42
RUN mvn package
CMD /bin/sh
