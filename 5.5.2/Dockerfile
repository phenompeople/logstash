#Base image
FROM phenompeople/centos-sunjre:latest
MAINTAINER Rajesh Jonnalagadda "admin.squad@phenompeople.com"
LABEL Description="Logstash Docker image based on Centos 7" \
	  License="Apache License 2.0" \
	  Version="5.5.2" \
	  project="logstash"
ARG PACKAGE_VERSION=5.5.2
ENV container docker \
    PACKAGE_VERSION=${PACKAGE_VERSION}
EXPOSE 5004
ADD logstash.repo /etc/yum.repos.d/logstash.repo
RUN yum install -y -q logstash-${PACKAGE_VERSION}-1 && \
    rm -rf /etc/yum.repos.d/logstash.repo && \
    yum clean all
COPY setup/config/log4j2.properties /etc/logstash/log4j2.properties
VOLUME /etc/logstash/conf.d
ENTRYPOINT ["/usr/share/logstash/bin/logstash", "--path.settings", "/etc/logstash"]
