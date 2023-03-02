FROM nginx:1.23
#RUN ! test -d /opt/configscripts || mkdir /opt/configscripts/
#COPY appconfig.tgz /opt/configscripts/
RUN apt-get update && apt-get install -y \
    python3 \
    python3-pip \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN ln -s /usr/bin/python3 /usr/bin/python 