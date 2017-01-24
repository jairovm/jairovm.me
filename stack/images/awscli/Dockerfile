FROM resin/rpi-raspbian:jessie

RUN apt-get update \
    && apt-get install -y python python-pip \
    && pip install awscli \
    && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

ENTRYPOINT ["/usr/local/bin/aws"]
