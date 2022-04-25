

FROM quay.io/centos/centos:stream8

MAINTAINER adevur (madavurro@protonmail.com)

RUN (curl -sL https://rpm.nodesource.com/setup_18.x | bash -) \
  && yum clean all -y \
  && yum update -y \
  && yum install -y nodejs \
  && yum autoremove -y \
  && yum clean all -y \
  && npm install npm --global

