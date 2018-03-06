FROM jenkins/jenkins:lts

USER root

#RUN apt-get update && \
#    apt-get -y install software-properties-common && \
#    apt-add-repository -y ppa:ansible/ansible && \
#    apt-get update && \
#    apt-get -y install ansible

RUN apt-get update && \
    apt install -y python-pip libssl-dev make gcc && \
    pip install -U pip setuptools wheel && \
    pip install ansible

USER jenkins
