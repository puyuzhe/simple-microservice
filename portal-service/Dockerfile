FROM java:8-jdk-alpine

MAINTAINER pyz

COPY target/portal-service.jar .

CMD java -jar portal-service.jar --spring.profiles.active=fat
