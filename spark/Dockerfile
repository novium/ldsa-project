FROM bde2020/hadoop-base:2.0.0-hadoop3.2.1-java8

ENV SPARK_VERSION=2.4.5

RUN apt-get update && apt-get install curl bash openjdk8-jre python3 py-pip nss libc6-compat \
      && ln -s /lib64/ld-linux-x86-64.so.2 /lib/ld-linux-x86-64.so.2 \
      && chmod +x *.sh \
      && wget https://archive.apache.org/dist/spark/spark-${SPARK_VERSION}/spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
      && tar -xvzf spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
      && mv spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION} spark \
      && rm spark-${SPARK_VERSION}-bin-hadoop${HADOOP_VERSION}.tgz \
      #&& cd /css \
      #&& jar uf /spark/jars/spark-core_2.11-${SPARK_VERSION}.jar org/apache/spark/ui/static/timeline-view.css \
      && cd /

ENV PYTHONHASHSEED 1
