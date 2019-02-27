FROM fedora:27
RUN dnf -y install krb5-workstation vim procps passwd authconfig pam_krb5
RUN mkdir /opt/docker
COPY  * /opt/docker/
WORKDIR /opt/docker
RUN chmod +x /opt/docker/startup.sh /opt/docker/install.sh
CMD ["/opt/docker/startup.sh"]

