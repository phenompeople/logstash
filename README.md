[![Docker Automated build](https://img.shields.io/docker/automated/phenompeople/logstash.svg?style=plastic)](https://hub.docker.com/r/phenompeople/logstash/)
[![Docker Build Status](https://img.shields.io/docker/build/phenompeople/logstash.svg?style=plastic)](https://hub.docker.com/r/phenompeople/logstash/)
[![Docker Pulls](https://img.shields.io/docker/pulls/phenompeople/logstash.svg?style=plastic)](https://hub.docker.com/r/phenompeople/logstash/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Logstash 

Dockerfiles for building Centos based Logstash images.

## Supported tags and respective Dockerfile links

### phenompeople/logstash

* **`latest`   ([6.1.2/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/6.1.2/Dockerfile))**
* **`6.1.2` 		([6.1.2/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/6.1.2/Dockerfile))**
* **`5.6.2` 		([5.6.2/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/5.6.2/Dockerfile))**
* **`5.5.2` 		([5.5.2/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/5.5.2/Dockerfile))**
* **`5.4.1` 		([5.4.1/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/5.4.1/Dockerfile))**
* **`5.3.0` 		([5.3.0/Dockerfile](https://bitbucket.org/phenompeople/logstash/src/master/5.3.0/Dockerfile))**

### Pre-Requisites

- install docker-engine [https://docs.docker.com/engine/installation/](https://docs.docker.com/engine/installation/)

## How to use this image 

1.  This image can be used by simply running 

```$ docker run --name=logstash -p 5004:5004 -v /etc/logstash/conf.d:/etc/logstash/conf.d -td phenompeople/logstash```

Above command runs logstash container with port 5004 mapped to host and reading configuration files mapped under /etc/logstash/conf.d. 

1. To make image run even after reboot use extra option --restart=always

```$ docker run --restart=always --name=logstash -p 5004:5004 -v /etc/logstash/conf.d:/etc/logstash/conf.d -td phenompeople/logstash```

## Maintainers

* Rajesh Jonnalagadda (<rajesh.jonnalagadda@phenompeople.com>)

## License and Authors

**License:**	Apache License

**Author :** Phenompeople Pvt Ltd (<admin.squad@phenompeople.com>)