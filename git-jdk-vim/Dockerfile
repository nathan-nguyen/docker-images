FROM ubuntu:latest

ENV DEBIAN_FRONTEND=noninteractive

# Update and install required packages: git, JDK, and vim
RUN apt-get update && apt-get install -y \
    git \
    openjdk-11-jdk \
    vim \
 && apt-get clean && rm -rf /var/lib/apt/lists/*

ENV JAVA_HOME=/usr/lib/jvm/java-11-openjdk-amd64
ENV PATH="$JAVA_HOME/bin:$PATH"

RUN git --version && \
    java -version && \
    vim --version

# Set the default command to bash
CMD ["/bin/bash"]
