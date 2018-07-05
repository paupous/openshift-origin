FROM ubuntu:16.04

RUN apt-get update -y \
    && apt-get install curl -y python-pip jq dos2unix \    
    && pip install yq 

RUN apt-get install gettext-base -y
    
RUN curl -s -L https://github.com/openshift/origin/releases/download/v3.9.0/openshift-origin-client-tools-v3.9.0-191fece-linux-64bit.tar.gz -o /tmp/oc.tar.gz \
    && tar zxvf /tmp/oc.tar.gz -C /tmp/ \
    && cp /tmp/openshift-origin-client-tools-v3.9.0-191fece-linux-64bit/oc /usr/local/bin/
    