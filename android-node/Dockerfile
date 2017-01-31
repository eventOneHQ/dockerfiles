FROM filiosoft/jdk-node:latest
MAINTAINER Filiosoft <Team@Filiosoft.com>

ENV TOOLS_VERSION 25.2.3
ENV TOOLS_ZIP "tools_r${TOOLS_VERSION}-linux.zip"
ENV AP_FILE "https://git.io/vDtRc"
ENV AP_OUT "android_packages.txt"
ENV ANDROID_HOME "/opt/android-sdk-linux"
ENV PATH "${PATH}:${ANDROID_HOME}/tools/bin:${ANDROID_HOME}/platform-tools:${ANDROID_HOME}/tools"

RUN apt-get -qq update && \
    apt-get -y --no-install-recommends install lib32stdc++6 lib32z1 && \
    apt-get -y autoremove && \
    apt-get -y autoclean && \
    rm -rf /var/lib/apt/lists/* 

RUN curl -s -O https://dl.google.com/android/repository/${TOOLS_ZIP} && \
    unzip -q ${TOOLS_ZIP} -d ${ANDROID_HOME}

RUN wget ${AP_FILE} -O ${AP_OUT} -q && \
    echo y | sdkmanager --package_file=${AP_OUT}
    
RUN sdkmanager --list && \
    rm -rf ${TOOLS_ZIP} ${AP_OUT}