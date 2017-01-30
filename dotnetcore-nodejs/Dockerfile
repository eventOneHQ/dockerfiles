FROM microsoft/dotnet
MAINTAINER Filiosoft Team <team@filiosoft.com>

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash - && \
    apt-get install -y nodejs && \
    apt-get install -y libssl-dev libffi-dev && \
    apt-get install -y python-dev && \
    apt-get install -y build-essential && \
    curl -L https://aka.ms/InstallAzureCli | bash && \
    npm i -g bower && \
    apt-get clean