FROM java:8
ADD open-eureka-server-1.0-SNAPSHOT.jar open-eureka-server.jar
RUN sh -c 'touch /open-eureka-server.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java -Xmx64M $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /open-eureka-server.jar" ]