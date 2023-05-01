FROM ubuntu:latest

RUN apt install -y \
    sudo bash wget locales

RUN localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8

RUN useradd coder --create-home --shell=/bin/bash --uid=1000 --user-group -p "$(openssl passwd -1 password)" && \
    echo "coder ALL=(ALL) NOPASSWD:ALL" >>/etc/sudoers.d/nopasswd

USER 1000
WORKDIR /home/coder

ENV LANG="en_US.UTF-8"
