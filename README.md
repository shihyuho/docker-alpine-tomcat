## Minified Docker image with Tomcat, Java with unlimited JCE patch applied

[![Build Status](https://travis-ci.org/davidcaste/docker-alpine-tomcat.svg?branch=master)](https://travis-ci.org/davidcaste/docker-alpine-tomcat)

[![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:latest.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:latest)

Basic [Docker](https://www.docker.com/) image to run [Tomcat](https://tomcat.apache.org/) and [Java](https://www.java.com/) with unlimited JCE patch applied.

This image is based on [AlpineLinux](http://alpinelinux.org/) to keep the size dow, yet smaller images do exist. Includes BASH, since many Java applications like to have convoluted BASH start-up scripts.

Extends [`davidcaste/alpine-java-unlimited-jce`](https://hub.docker.com/r/davidcaste/alpine-java-unlimited-jce/).


### Versions

**Tomcat 8 Version**: `8.0.32`  
**Tomcat 7 Version**: `7.0.68`  
**JRE8/JDK8 Version**: `8u74-b02`  
**JRE7/JDK7 Version**: `7u80-b15`

### Tags

| Tomcat version | Java version      | tags                           | Size                                                                                                                                              |
|:---------------|:------------------|:-------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------|
| Tomcat 8       | Oracle Java 8 JRE | latest / tomcat8 / jre8tomcat8 | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jre8tomcat8.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jre8tomcat8) |
| Tomcat 8       | Oracle Java 8 JDK | jdk8tomcat8                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jdk8tomcat8.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jdk8tomcat8) |
| Tomcat 8       | Oracle Java 7 JRE | jre7tomcat8                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jre7tomcat8.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jre7tomcat8) |
| Tomcat 8       | Oracle Java 7 JDK | jdk7tomcat8                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jdk7tomcat8.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jdk7tomcat8) |
| Tomcat 7       | Oracle Java 8 JRE | tomcat7 / jre8tomcat7          | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jre8tomcat7.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jre8tomcat7) |
| Tomcat 7       | Oracle Java 8 JDK | jdk8tomcat7                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jdk8tomcat7.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jdk8tomcat7) |
| Tomcat 7       | Oracle Java 7 JRE | jre7tomcat7                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jre7tomcat7.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jre7tomcat7) |
| Tomcat 7       | Oracle Java 7 JDK | jdk7tomcat7                    | [![](https://badge.imagelayers.io/davidcaste/alpine-tomcat:jdk7tomcat7.svg)](https://imagelayers.io/?images=davidcaste/alpine-tomcat:jdk7tomcat7) |


### Usage

Example:

    docker run -it --rm davidcaste/alpine-tomcat java -version
