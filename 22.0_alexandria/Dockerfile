FROM ubuntu:18.04
RUN apt update -y && \
    apt upgrade -y && \
    apt install -y curl && \
    apt autoclean -y && \
    apt autoremove -y
RUN apt install -y joe wget p7zip-full curl openssh-server build-essential zlib1g-dev libcurl4-gnutls-dev libncurses5
COPY LinuxPAServer22.0.tar.gz ./
RUN tar -xvf LinuxPAServer22.0.tar.gz
ENTRYPOINT ./PAServer-22.0/paserver -password=


