FROM jupyter/base-notebook

USER root

RUN apt-get update && \
    apt-get install -y default-jre wget unzip

RUN wget https://github.com/NetLogo/NetLogo/releases/download/7.0.3/NetLogo-7.0.3-64.tgz && \
    tar -xzf NetLogo-7.0.3-64.tgz && \
    mv NetLogo\ 7.0.3 /opt/netlogo

USER $NB_UID
