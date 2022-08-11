FROM java:11
VOLUME /tmp
Add demo1-0.0.1-SNAPSHOT.jar demo1-0.0.1-SNAPSHOT.jar
EXPOSE 8080
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/demo1.jar"]