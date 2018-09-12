#FROM tomcat:7-jre8-alpine
FROM davidcaste/alpine-tomcat:tomcat7

ADD https://nexus.ideaconsult.net/content/repositories/releases/ambit/ambit2-www/3.1.0/ambit2-www-3.1.0.war /opt/tomcat/webapps/ambit.war

ENTRYPOINT ["/opt/tomcat/bin/catalina.sh", "run"]
