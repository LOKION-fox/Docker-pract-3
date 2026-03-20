FROM ubuntu:latest

RUN apt-get update && apt-get install -y \
    xterm \
    xauth \
    && rm -rf /var/lib/apt/lists/*

ENV DISPLAY=host.docker.internal:0

CMD ["xterm", "-hold", "-e", "ls -la /"]