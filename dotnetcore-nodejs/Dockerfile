FROM microsoft/dotnet
MAINTAINER Filiosoft Team <team@filiosoft.com>

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash - 
RUN apt-get install -y nodejs libssl-dev libffi-dev python-dev build-essential
RUN curl -L https://aka.ms/InstallAzureCli | bash
RUN npm i -g bower 

RUN rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    apt-get purge -y --auto-remove $buildDeps && \
    apt-get autoremove -y && apt-get clean