FROM jenkins
USER root
RUN /usr/local/bin/install-plugins.sh docker-slaves gradle:1.25
RUN /usr/local/bin/install-plugins.sh docker-slaves git:3.0.0
RUN /usr/local/bin/install-plugins.sh docker-slaves git-client:2.0.0
RUN /usr/local/bin/install-plugins.sh docker-slaves job-import-plugin:1.5
RUN /usr/local/bin/install-plugins.sh docker-slaves saferestart:0.3
#USER jenkins # drop back to the regular jenkins user - good practice
