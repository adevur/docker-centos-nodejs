

FROM centos:7

MAINTAINER adevur (madavurro@protonmail.com)

RUN yum clean all -y \
  && yum update -y \
  && yum install -y curl \
  && (curl -sL https://rpm.nodesource.com/setup_10.x | bash -) \
  && yum install -y nodejs \
  && yum autoremove -y \
  && yum clean all -y \
  && npm install npm --global

