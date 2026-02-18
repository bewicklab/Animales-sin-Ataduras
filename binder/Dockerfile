FROM jupyter/base-notebook:lab-4.0.7

USER root

RUN apt-get update && \
    apt-get install -y default-jre wget unzip xvfb

RUN wget https://ccl.northwestern.edu/netlogo/6.3.0/NetLogo-6.3.0.tgz && \
    tar -xzf NetLogo-6.3.0.tgz && \
    mv NetLogo\ 6.3.0 /opt/netlogo

ENV NETLOGO_HOME=/opt/netlogo
ENV PATH=$NETLOGO_HOME:$PATH

USER $NB_UID
