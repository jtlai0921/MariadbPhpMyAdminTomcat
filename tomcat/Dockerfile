FROM tomcat:8.5.49-jdk8-openjdk

ADD ./conf/tomcat-users.xml $CATALINA_HOME/conf/

#USER root
ENV TZ=Asia/Taipei
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone


