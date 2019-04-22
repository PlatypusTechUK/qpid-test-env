FROM centos:7
RUN yum -y update && yum -y install epel-release && yum -y install qpid-cpp-server qpid-tools
WORKDIR /opt
COPY certs /opt/certs
EXPOSE 5671
EXPOSE 5672
EXPOSE 8080
CMD ["/usr/sbin/qpidd", "--ssl-cert-password-file", "/opt/certs/passwd.txt", "--ssl-cert-db", "/opt/certs/", "--ssl-cert-name", "qpidd", "--mgmt-enable", "yes", "--mgmt-publish", "yes"]
