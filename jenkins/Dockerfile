FROM jenkins
USER root
RUN /usr/local/bin/install-plugins.sh docker-slaves gradle:1.25
USER jenkins # drop back to the regular jenkins user - good practice
