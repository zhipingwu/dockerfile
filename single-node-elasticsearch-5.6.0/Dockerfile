FROM openjdk:8

MAINTAINER wzp

ADD elasticsearch-5.6.0.zip /elasticsearch-5.6.0.zip
RUN unzip /elasticsearch-5.6.0.zip
RUN useradd es
RUN chown es -R /elasticsearch-5.6.0
USER es
EXPOSE 9200
EXPOSE 9300

CMD /elasticsearch-5.6.0/bin/elasticsearch
