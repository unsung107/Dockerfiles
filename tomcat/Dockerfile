FROM openjdk:11-jre-slim
MAINTAINER Foo Bar <foo@bar.com>

RUN apt-get update
RUN apt-get -y install wget

WORKDIR /usr/local/
RUN wget http://mirror.apache-kr.org/tomcat/tomcat-9/v9.0.38/bin/apache-tomcat-9.0.38.tar.gz
RUN tar xvzf apache-tomcat-9.0.38.tar.gz
RUN rm -f apache-tomcat-9.0.38.tar.gz

EXPOSE 8080

CMD /usr/local/apache-tomcat-9.0.38/bin/catalina.sh run
