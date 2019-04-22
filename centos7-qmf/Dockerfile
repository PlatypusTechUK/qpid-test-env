FROM centos:7
RUN yum -y update && yum -y install epel-release && yum -y install java && yum -y clean all
WORKDIR /opt
COPY qpid-qmf2-tools . 
EXPOSE 8080
CMD ["/opt/qpid-qmf2-tools/bin/QpidRestAPI.sh"]
