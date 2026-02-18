FROM openjdk:11-jre-slim

RUN apt-get update && apt-get install -y wget unzip && rm -rf /var/lib/apt/lists/*

# Install NetLogo Headless
RUN wget https://github.com/NetLogo/NetLogo/releases/download/v6.4.0/NetLogo-6.4.0-64.tgz \
    && tar -xzf NetLogo-6.4.0-64.tgz \
    && mv NetLogo\ 6.4.0 /opt/netlogo \
    && rm NetLogo-6.4.0-64.tgz

ENV PATH="/opt/netlogo:${PATH}"
