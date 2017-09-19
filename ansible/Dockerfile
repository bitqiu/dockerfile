FROM bitqiu/ubuntu:latest

RUN apt-get update -y && \
    apt-get install -y software-properties-common && \
    apt-add-repository ppa:ansible/ansible && \
    apt-get update -y && \
    apt-get install -y ansible && \
    echo 'localhost' > /etc/ansible/hosts && \
    rm -rf /var/lib/apt/lists/* && \
    apt-get clean

CMD ["/usr/bin/ansible"]