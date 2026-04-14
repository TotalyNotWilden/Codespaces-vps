
FROM ubuntu:22.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    xfce4 \
    xfce4-goodies \
    firefox \
    sudo \
    curl \
    git \
    && apt-get clean && rm -rf /var/lib/apt/lists/*


RUN useradd -m -s /bin/bash codespace && \
    echo "codespace ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers
