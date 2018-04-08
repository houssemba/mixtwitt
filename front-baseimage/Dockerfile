FROM debian:latest

RUN apt-get update && \
    apt-get upgrade -y

RUN apt-get install  -y apache2

# Clean up
RUN apt-get autoremove
RUN apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

# Expose the port for usage with the docker -P switch
EXPOSE 80

# Run Apache 2
CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]
