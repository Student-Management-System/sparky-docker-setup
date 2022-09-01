FROM openjdk:17-jdk-bullseye
RUN mkdir -p /opt/registry
WORKDIR /opt/registry

ADD https://jenkins-2.sse.uni-hildesheim.de/view/Teaching/job/Teaching_Sparky-RuntimeServiceRegistry/lastSuccessfulBuild/artifact/target/registry.jar registry.jar
EXPOSE 8671
ENTRYPOINT ["java", "-jar", "registry.jar"] 