FROM centos:5

MAINTAINER Milan Sulc <sulcmil@gmail.com>

ENV TERM xterm
ENV USER_UID 1000
ENV USER_NAME dfx

RUN yum update -y && \
    yum upgrade -y && \
    useradd -ms /bin/bash -u $USER_UID $USER_NAME && \
    yum clean all && \
    rm -rf /tmp/* /var/tmp/*

CMD ["/bin/bash"]
