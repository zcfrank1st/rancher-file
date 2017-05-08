FROM openjdk:8

WORKDIR /opt

RUN apt-get install -y wget \
    && apt-get install -y unzip \
    && wget http://apache.claz.org/incubator/rocketmq/4.0.0-incubating/rocketmq-all-4.0.0-incubating-bin-release.zip \
    && unzip rocketmq-all-4.0.0-incubating-bin-release.zip \
    && echo "ROCKETMQ_HOME=/opt/apache-rocketmq-all" >> ~/.bashrc \
    && echo "PATH=$ROCKETMQ_HOME/bin:$PATH" >> ~/.bashrc \
    && /bin/bash -c "source ~/.bashrc"
