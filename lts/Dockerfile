

FROM quay.io/centos/centos:stream8

MAINTAINER Luca Polito (info.lucapolito@yahoo.it)

RUN (curl -sL https://rpm.nodesource.com/setup_16.x | bash -) \
  && yum clean all -y \
  && yum update -y \
  && yum install -y nodejs \
  && yum autoremove -y \
  && yum clean all -y \
  && npm install npm --global

