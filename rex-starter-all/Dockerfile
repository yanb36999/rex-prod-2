FROM java:8

COPY target/rex-starter-all.jar /app.jar
COPY rex-ui/ /rex-ui/
COPY hosts /etc/hosts
EXPOSE 8080
ENTRYPOINT ["java","-jar","-server","-Xms2g","-Xmx2g","-Xmn1g","-XX:+UseG1GC","-XX:SurvivorRatio=6","/app.jar"]
