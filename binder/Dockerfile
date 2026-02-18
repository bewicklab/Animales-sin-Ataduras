FROM jupyter/base-notebook

USER root

RUN apt-get update && \
    apt-get install -y default-jre wget unzip

RUN wget https://github.com/NetLogo/NetLogo/releases/download/6.3.0/NetLogo-6.3.0-64.tgz && \
    tar -xzf NetLogo-6.3.0-64.tgz && \
    mv NetLogo\ 6.3.0 /opt/netlogo
    
USER $NB_UID
