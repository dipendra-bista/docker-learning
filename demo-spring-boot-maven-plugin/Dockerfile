FROM openjdk:8-jre
VOLUME /tmp
EXPOSE 8081
ADD target/*.jar app.jar
ENTRYPOINT ["sh","-c" ,"java -jar /app.jar"]

# Add Maven dependencies (not shaded into the artifact; Docker-cached)
#ADD target/lib           /usr/share/myservice/lib

# Add the service itself

#ARG JAR_FILE
#ADD target/${JAR_FILE} /usr/share/myservice/myservice.jar