FROM openjdk:latest

RUN apt-get update && \
    apt-get upgrade -y

# Clean up
RUN apt-get autoremove
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
