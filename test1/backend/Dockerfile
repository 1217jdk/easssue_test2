#FROM gradle:7.5
FROM zaq1290/spring_konlpy

WORKDIR /var/jenkins_home/workspace/backend/backend

COPY ./ ./

RUN gradle clean build --no-daemon

ENTRYPOINT ["java", "-jar", "./build/libs/easssue-0.0.1-SNAPSHOT.jar"]
