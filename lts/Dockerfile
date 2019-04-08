

FROM centos:7

MAINTAINER adevur (madavurro@protonmail.com)

RUN yum clean all -y \
  && yum update -y \
  && yum install -y curl \
  && yum autoremove -y

RUN curl -sL https://rpm.nodesource.com/setup_10.x | bash -

RUN yum clean all -y \
  && yum install -y nodejs

RUN npm install npm --global

