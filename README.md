[![dockeri.co](http://dockeri.co/image/phenompeople/logstash)](https://registry.hub.docker.com/phenompeople/logstash/)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Logstash 

Dockerfiles for building Centos based Logstash images.

## Supported tags and respective Dockerfile links

### phenompeople/logstash

* **`latest`    ([7.6.0/Dockerfile](https://github.com/phenompeople/logstash/blob/master/7.2.0/Dockerfile))**
* **`7.6.0`    ([7.6.0/Dockerfile](https://github.com/phenompeople/logstash/blob/master/7.6.0/Dockerfile))**
* **`7.2.0`     ([7.2.0/Dockerfile](https://github.com/phenompeople/logstash/blob/master/7.2.0/Dockerfile))**
* **`6.8.0` 	([6.8.0/Dockerfile](https://github.com/phenompeople/logstash/blob/master/6.8.0/Dockerfile))**
* **`6.5.0` 	([6.5.0/Dockerfile](https://github.com/phenompeople/logstash/blob/master/6.5.0/Dockerfile))**

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
* Harshavardhan Baddam (<harshavardhan.baddam@phenompeople.com>)

## License and Authors

**License:**	Apache License

**Author :** Phenompeople Pvt Ltd (<admin.squad@phenompeople.com>)