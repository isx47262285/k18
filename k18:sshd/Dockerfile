FROM fedora:27
LABEL author="@robert72004 ASIX M11-SAD"
LABEL description="SSH server"
RUN dnf -y install krb5-workstation vim procps openssh-clients openssh-server passwd 
RUN mkdir /opt/docker
COPY  * /opt/docker/
WORKDIR /opt/docker
RUN chmod +x /opt/docker/startup.sh /opt/docker/install.sh
CMD ["/opt/docker/startup.sh"]

