FROM docker.io/maven:adoptopenjdk
LABEL org.opencontainers.image.source https://github.com/skhedim/cloud-native-epsi

COPY pom.xml .
COPY src ./src

RUN mvn verify

EXPOSE 8080

ENTRYPOINT ["java", "-Xmx8m", "-Xms8m", "-jar", "/target/words.jar"]