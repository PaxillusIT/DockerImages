FROM centos:7

RUN yum -y group install "Development Tools"; \
    yum install epel-release -y; \
    yum install ansible -y; \
    yum -y install python-devel krb5-devel krb5-libs krb5-workstation; \
    yum -y install python-pip; \
    yum -y install bind-utils; \
    yum -y update; \
    yum clean all;

RUN pip install --upgrade pip; \
    pip install pywinrm[Kerberos]; \
    pip install xmltodict; 