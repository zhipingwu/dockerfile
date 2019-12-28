FROM  openjdk:8

#维护者
MAINTAINER zhipingwu

# 运行之前最好先下载到本地然后copy
# wget http://mirror.bit.edu.cn/apache/hbase/hbase-1.3.6/hbase-1.3.6-bin.tar.gz
# wget http://mirror.bit.edu.cn/apache/phoenix/apache-phoenix-4.14.2-HBase-1.3/bin/apache-phoenix-4.14.2-HBase-1.3-bin.tar.gz

ADD hbase-1.3.6-bin.tar.gz /usr/local/hadoop/hbase
ADD apache-phoenix-4.14.2-HBase-1.3-bin.tar.gz /usr/local/hadoop/hbase/phoenix
RUN cp /usr/local/hadoop/hbase/phoenix/apache-phoenix-4.14.2-HBase-1.3/*.jar /usr/local/hadoop/hbase/hbase-1.3.6-bin/lib/
RUN echo "export JAVA_HOME=/usr/local/openjdk-8" >> /usr/local/hadoop/hbase/hbase-1.3.6/conf/hbase-env.sh

EXPOSE 2181
#设置启动命令
CMD /usr/local/hadoop/hbase/hbase-1.3.6/bin/start-hbase.sh && sleep 999999999999
