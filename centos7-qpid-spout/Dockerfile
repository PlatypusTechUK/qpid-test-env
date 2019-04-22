FROM centos:7
#RUN yum -y update && yum -y install git epel-release && yum -y install cmake boost-devel libuuid-devel pkgconfig gcc-c++ make ruby help2man doxygen graphviz cyrus-sasl-devel cyrus-sasl-md5 cyrus-sasl-plain nss-devel nspr-devel xqilla-devel xerces-c-devel libibverbs-devel librdmacm-devel 
RUN yum -y update && yum -y install git epel-release && yum -y install qpid-cpp-client-devel 
WORKDIR /opt
COPY certs /opt/certs
RUN mkdir /opt/data && mkdir /opt/bin
VOLUME /opt/data
