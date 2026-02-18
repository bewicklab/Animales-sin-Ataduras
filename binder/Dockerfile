FROM eclipse-temurin:11-jre-jammy

RUN apt-get update && \
    apt-get install -y wget unzip && \
    rm -rf /var/lib/apt/lists/*

WORKDIR /opt

RUN wget https://github.com/NetLogo/NetLogo/releases/download/6.2.2/NetLogo-6.2.2-64.tgz && \
    tar -xzf NetLogo-6.2.2-64.tgz && \
    mv NetLogo\ 6.2.2 netlogo

ENV NETLOGO_HOME=/opt/netlogo
ENV PATH=$NETLOGO_HOME:$PATH
