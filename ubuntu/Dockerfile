FROM ubuntu:16.04

RUN sed -i 's/archive.ubuntu.com/mirrors.ustc.edu.cn/g' /etc/apt/sources.list && \
    apt-get update -y && \
    apt-get install -y software-properties-common vim.tiny wget sudo net-tools ca-certificates unzip apt-transport-https && \
    rm -rf /var/lib/apt/lists/* && \
    apt-get clean