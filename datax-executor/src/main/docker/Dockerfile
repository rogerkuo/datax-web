FROM ibbd/java-python3:latest

LABEL maintainer="rogerkuo"

RUN apt-get install -y wget \
    && mkdir /datax \
    && wget -O /datax/datax.tar.gz  "http://datax-opensource.oss-cn-hangzhou.aliyuncs.com/datax.tar.gz" \
    && tar -xvf /datax/datax.tar.gz

ENV DATAX_HOME=/var/www/datax
ENV PATH $PATH:$DATAX_HOME/bin