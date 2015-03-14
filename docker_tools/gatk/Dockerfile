FROM java

RUN apt-get update
RUN apt-get install -y mvn git

RUN cd home/
RUN git clone https://github.com/broadgsa/gatk-protected/
RUN cd gatk-protected/
RUN mvn package
RUN mv target/GenomeAnalysisTK.jar /home