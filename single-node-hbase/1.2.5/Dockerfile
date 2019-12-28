FROM  openjdk:8

#维护者
MAINTAINER zhipingwu

# 运行之前最好先下载到本地然后copy
# wget http://archive.apache.org/dist/hbase/1.2.5/hbase-1.2.5-bin.tar.gz
# wget http://archive.apache.org/dist/phoenix/apache-phoenix-4.13.1-HBase-1.2/bin/apache-phoenix-4.13.1-HBase-1.2-bin.tar.gz

RUN wget http://archive.apache.org/dist/hbase/1.2.5/hbase-1.2.5-bin.tar.gz
RUN wget http://archive.apache.org/dist/phoenix/apache-phoenix-4.13.1-HBase-1.2/bin/apache-phoenix-4.13.1-HBase-1.2-bin.tar.gz
RUN tar zxvf hbase-1.2.5-bin.tar.gz -C /usr/local/hadoop/hbase
RUN ls /usr/local/hadoop/hbase/hbase-1.2.5
RUN echo "export JAVA_HOME=/usr/local/openjdk-8" >> /usr/local/hadoop/hbase/hbase-1.2.5/conf/hbase-env.sh

EXPOSE 2181
#设置启动命令
CMD /usr/local/hadoop/hbase/hbase-1.3.6/bin/start-hbase.sh && sleep 999999999999
