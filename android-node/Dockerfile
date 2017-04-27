FROM filiosoft/jdk-node:latest
MAINTAINER Filiosoft <Team@Filiosoft.com>

ENV TOOLS_VERSION 3859397
ENV TOOLS_ZIP "sdk-tools-linux-${TOOLS_VERSION}.zip"
ENV AP_FILE "https://git.io/vDtRc"
ENV AP_OUT "android_packages.txt"
ENV ANDROID_HOME "/opt/android-sdk-linux"
ENV GRADLE_VER 3.5
ENV GRADLE_HOME "/opt/gradle"
ENV GRADLE_ZIP "gradle-${GRADLE_VER}-bin.zip"
ENV PATH "${PATH}:${ANDROID_HOME}/tools/bin:${ANDROID_HOME}/platform-tools:${ANDROID_HOME}/tools:${GRADLE_HOME}/gradle-${GRADLE_VER}/bin"

RUN apt-get -qq update && \
    apt-get -y --no-install-recommends install lib32stdc++6 lib32z1 && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 

RUN curl -s -O https://dl.google.com/android/repository/${TOOLS_ZIP} && \
    wget https://services.gradle.org/distributions/${GRADLE_ZIP} -q && \
    unzip -q ${TOOLS_ZIP} -d ${ANDROID_HOME} && \
    unzip -q ${GRADLE_ZIP} -d ${GRADLE_HOME}

RUN wget ${AP_FILE} -O ${AP_OUT} -q && \
    echo y | sdkmanager --package_file=${AP_OUT}
    
RUN sdkmanager --list && \
    rm -rf ${TOOLS_ZIP} ${AP_OUT} ${GRADLE_ZIP}
