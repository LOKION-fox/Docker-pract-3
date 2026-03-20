FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    openjdk-17-jre \
    x11-apps \
    xauth \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /app
COPY calc.jar /app/calc.jar

ENV DISPLAY=host.docker.internal:0

CMD ["java", "-jar", "/app/calc.jar"]