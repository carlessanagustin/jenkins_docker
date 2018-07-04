FROM jenkins/jenkins:lts

USER root

RUN apt-get update && \
    apt-get -y install software-properties-common apt-transport-https libssl-dev make gcc && \
    apt-get -y install python-pip python-setuptools python-wheel

#RUN apt-add-repository -y ppa:ansible/ansible && \
#    apt-get update && \
#    apt-get -y install ansible

RUN pip install ansible
RUN pip install boto apache-libcloud

# configuration...
# https://docs.ansible.com/ansible/latest/scenario_guides/guide_gce.html
# https://docs.ansible.com/ansible/latest/scenario_guides/guide_aws.html

USER jenkins

