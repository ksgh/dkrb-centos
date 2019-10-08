FROM scratch
ADD 8/centos-8-container.tar.xz /

LABEL org.label-schema.schema-version="1.0" \
    org.label-schema.name="CentOS Base Image" \
    org.label-schema.vendor="CentOS" \
    org.label-schema.license="GPLv2" \
    org.label-schema.build-date="20190927"

ENV LANG=en_US.UTF-8 \
    LANGUAGE=en_US.UTF-8

RUN yum update -y && \
    yum install -y \
        epel-release \
        bind-utils \
        which && \
    yum clean all

ENTRYPOINT []
CMD ["/bin/bash"]
