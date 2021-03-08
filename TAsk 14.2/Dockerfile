FROM centos:latest
RUN yum install net-tools openssh-server passwd -y
RUN ssh-keygen -A
RUN echo redhat | passwd root --stdin
EXPOSE 22
CMD ["/usr/sbin/sshd","-D"]

