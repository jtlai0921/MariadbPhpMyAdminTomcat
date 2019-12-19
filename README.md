# Mariadb Tomcat Docker environment
## Description 
* This is a developer environment with mariadb , tomcat , phpMyAdmin  docker

## Gettting started
* install docker , docker-compose
* cd directory and `sudo docker-compose up -d --build` to run environment
* execute you sql script with phpMyAdmin
* project complie and build  war put into  tomcat-webapps
* browser `http://yourip:8080/warFileName` 

## docker information
* mariadb : latest
* phpMyadmin : latest
* tomcat : 8.5.49-jdk8-openjdk

## information
* tomcat with manager/html default account /pwd `admin / mypassword112233`
* mariadb root default password `myadmin123` 
* phpMyAdmin default port `8088`
* tomcat default port `8080` ajp port `8009`
* `tomcat-webapps/` you can put your war file or project directory

```ssh
docker build -t jenkinsagent:maven3.5 .

docker run \
    --name jenkins_maven_agent \
    -d --restart always \
    jenkinsagent:maven3.5 \
    -url http://10.0.2.15:8080 \
    c11d83024cd7b90b290545c0748c5777bd92d35fa9cd83bdbc6b44f5afc43f5f \
    maven_agent 
```
