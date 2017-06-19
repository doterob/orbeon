FROM tomcat:8-jre8-alpine

ADD https://github.com/orbeon/orbeon-forms/releases/download/tag-release-2016.3-ce/orbeon-2016.3.201612302139-CE.zip /tmp
ADD https://jdbc.postgresql.org/download/postgresql-42.1.1.jar $CATALINA_HOME/lib

RUN unzip /tmp/orbeon-2016.3.201612302139-CE.zip -d /tmp &&\
	mv /tmp/orbeon-2016.3.201612302139-CE $CATALINA_HOME/webapps/orbeon 

ADD context.xml $CATALINA_HOME/webapps/orbeon/META-INF/context.xml

