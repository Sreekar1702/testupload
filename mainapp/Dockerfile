#FROM openjdk:11
#ARG JAR_FILE=target/*.jar
#COPY ${JAR_FILE} mainapp.jar
#ENTRYPOINT ["java","-jar","/mainapp.jar"]
#EXPOSE 9001
FROM openjdk:11
RUN mkdir -p /home/docker_user/app/
RUN chmod 755 /home/docker_user/app/
COPY target/mainapp-0.0.1-SNAPSHOT.jar /home/docker_user/app/mainapp.jar
EXPOSE 9001
CMD ["java","-jar","/home/docker_user/app/mainapp.jar"]