FROM openjdk:8-jdk-stretch
RUN apt-get update && apt-get install maven -y maven && apt-get install git -y git
WORKDIR /home
RUN git clone https://github.com/kupa2004/App42.git
WORKDIR /home/App42
RUN mvn package
CMD /bin/sh
