FROM mcr.microsoft.com/devcontainers/base:ubuntu-24.04

# Install Docker dependencies and tools needed for Android Studio
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
    && apt-get -y install --no-install-recommends \
        wget \
        openjdk-17-jdk \
        android-tools-adb \
        android-tools-fastboot \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# Set JAVA_HOME
ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
