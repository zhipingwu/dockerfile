FROM  openjdk:8

#维护者
MAINTAINER zhipingwu

# 运行之前最好先下载到本地然后copy
# wget http://mirror.bit.edu.cn/apache/hbase/hbase-1.3.6/hbase-1.3.6-bin.tar.gz
ADD ./hbase-1.3.6-bin.tar.gz /usr/local/hadoop/hbase
RUN ls /usr/local/hadoop/hbase/hbase-1.3.6
RUN echo "export JAVA_HOME=/usr/local/openjdk-8" >> /usr/local/hadoop/hbase/hbase-1.3.6/conf/hbase-env.sh

EXPOSE 2181
#设置启动命令
CMD /usr/local/hadoop/hbase/hbase-1.3.6/bin/start-hbase.sh
