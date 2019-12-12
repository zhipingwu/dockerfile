FROM  openjdk:8

#维护者
MAINTAINER zhipingwu

# 运行之前最好先下载到本地然后copy
# wget http://mirrors.tuna.tsinghua.edu.cn/apache/kafka/2.1.1/kafka_2.11-2.1.1.tgz

ENV JAVA_HOME /usr/local/openjdk-8

ADD ./kafka_2.11-2.1.1.tgz /root/

EXPOSE 9092
#设置启动命令
CMD /root/kafka_2.11-2.1.1/bin/zookeeper-server-start.sh  /root/kafka_2.11-2.1.1/config/zookeeper.properties && /root/kafka_2.11-2.1.1/bin/kafka-server-start.sh /root/kafka_2.11-2.1.1/config/server.properties
