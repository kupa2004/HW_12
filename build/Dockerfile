FROM ubuntu:20.04
RUN apt-get update
RUN apt-get install default-jdk -y default-jdk && apt-get install maven -y maven && apt-get install git -y git
WORKDIR /home
RUN git clone https://github.com/shephertz/App42PaaS-Java-MySQL-Sample.git
WORKDIR App42PaaS-Java-MySQL-Sample/WebContent
RUN rm  Config.properties
#COPY /home/HW_12/config/Config.properties .
WORKDIR /home/App42PaaS-Java-MySQL-Sample
RUN mvn package
CMD /bin/sh
