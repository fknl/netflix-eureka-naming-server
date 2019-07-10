FROM openjdk:8-jdk

EXPOSE 8761

VOLUME /tmp
ADD maven/netflix-eureka-naming-server-0.0.1-SNAPSHOT.jar netflix-eureka-naming-server-0.0.1-SNAPSHOT.jar
RUN sh -c 'touch /netflix-eureka-naming-server-0.0.1-SNAPSHOT.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/netflix-eureka-naming-server-0.0.1-SNAPSHOT.jar"]
