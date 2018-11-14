FROM        openjdk:8u181-jdk

ENV         JAVA_HOME         /usr/lib/jvm/java-8-openjdk-amd64
ENV         GLASSFISH_HOME    /usr/local/glassfish5
ENV         PATH              $PATH:$JAVA_HOME/bin:$GLASSFISH_HOME/bin

RUN         apt-get update && \
            apt-get install -y curl unzip zip inotify-tools && \
            rm -rf /var/lib/apt/lists/*

RUN         curl -L -o /tmp/glassfish.zip https://download.oracle.com/glassfish/5.0.1/nightly/latest-glassfish.zip && \
            unzip /tmp/glassfish.zip -d /usr/local && \
            rm -f /tmp/glassfish.zip

EXPOSE      8080 4848 8181

WORKDIR     /usr/local/glassfish5

CMD         /usr/local/glassfish5/bin/asadmin start-domain --verbose