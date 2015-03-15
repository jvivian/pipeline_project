FROM java

RUN apt-get update
RUN apt-get install -y maven git

WORKDIR /home
RUN git clone https://github.com/broadgsa/gatk-protected/

WORKDIR /home/gatk-protected
RUN mvn package

RUN mv target/GenomeAnalysisTK.jar /home

WORKDIR /home