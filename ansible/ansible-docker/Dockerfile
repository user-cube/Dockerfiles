# ruicoelho43/ansible:latest
FROM debian:12

RUN apt-get update \
    && apt-get install --no-install-recommends -y python3-pip \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install pip --upgrade --break-system-packages
RUN pip3 install ansible --break-system-packages

RUN apt-get update -y && \
    DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
    sshpass

WORKDIR /work
