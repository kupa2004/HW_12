FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install git -y git && apt-get install default-jdk -y default-jdk && apt-get install maven -y maven
WORKDIR /home
RUN git clone https://github.com/kupa2004/App42.git
WORKDIR /home/App42
RUN mvn package
CMD /bin/sh
