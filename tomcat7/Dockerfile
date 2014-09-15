FROM dsw88/java7

RUN apt-get -y update && apt-get -y install wget

ENV CATALINA_HOME /tomcat

RUN wget --quiet "http://apache.arvixe.com/tomcat/tomcat-7/v7.0.55/bin/apache-tomcat-7.0.55.tar.gz"; \
    tar -xzf apache-tomcat-7.0.55.tar.gz; \
    rm -rf apache-tomcat-7.0.55.tar.gz; \
    mv apache-tomcat-7.0.55/ /tomcat; \
    rm -rf /tomcat/webapps/*
    
EXPOSE 8080

CMD ${CATALINA_HOME}/bin/catalina.sh run
    
