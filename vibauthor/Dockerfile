FROM centos:6
LABEL maintainer="https://keybase.io/tcely"

WORKDIR /root
RUN yum -y update && \
    curl -v -R -L -O 'http://download3.vmware.com/software/vmw-tools/vibauthor/vmware-esx-vib-author-5.0.0-0.0.847598.i386.rpm' && \
    yum -y install vmware-esx-vib-author-*.rpm && \
    rm -f vmware-esx-vib-author-*.rpm && \
    yum clean all
WORKDIR /data
ENTRYPOINT ["/usr/bin/vibauthor"]
CMD ["--help"]
