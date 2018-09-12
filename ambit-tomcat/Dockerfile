#FROM tomcat:7-jre8-alpine
FROM davidcaste/alpine-tomcat:tomcat7

RUN apk update \
    && apk add ca-certificates wget \
    && update-ca-certificates

#WORKDIR /usr/local/tomcat/webapps
WORKDIR /opt/tomcat/webapps
RUN ["wget", "-O", "ambit.war", "https://sourceforge.net/projects/ambit/files/Ambit2/AMBIT%20REST%20web%20services/services/ambit-rest-3.1.0/ambit.war/download?use_mirror=cfhcable"]

ENTRYPOINT ["/opt/tomcat/bin/catalina.sh", "run"]
