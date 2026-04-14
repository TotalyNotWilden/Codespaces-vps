
FROM ubuntu:24.04

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && apt-get install -y \
    xfce4 \
    xfce4-goodies \
    tightvncserver \
    xterm \
    sudo \
    curl \
    git \
    && apt-get clean

RUN useradd -m -s /bin/bash codespace && \
    echo "codespace:password" | chpasswd && \
    usermod -aG sudo codespace

EXPOSE 5901
