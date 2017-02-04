FROM buildpack-deps:jessie-scm
MAINTAINER Filiosoft Team <team@filiosoft.com>

# Install .NET CLI dependencies
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        libc6 \
        libcurl3 \
        libgcc1 \
        libgssapi-krb5-2 \
        libicu52 \
        liblttng-ust0 \
        libssl1.0.0 \
        libstdc++6 \
        libunwind8 \
        libuuid1 \
        zlib1g \
    && rm -rf /var/lib/apt/lists/*

# Install .NET Core SDK
ENV DOTNET_SDK_VERSION 1.0.0-rc3-004530
ENV DOTNET_SDK_DOWNLOAD_URL https://dotnetcli.blob.core.windows.net/dotnet/Sdk/$DOTNET_SDK_VERSION/dotnet-dev-debian-x64.$DOTNET_SDK_VERSION.tar.gz

RUN curl -SL $DOTNET_SDK_DOWNLOAD_URL --output dotnet.tar.gz \
    && mkdir -p /usr/share/dotnet \
    && tar -zxf dotnet.tar.gz -C /usr/share/dotnet \
    && rm dotnet.tar.gz \
    && ln -s /usr/share/dotnet/dotnet /usr/bin/dotnet

# Trigger the population of the local package cache
ENV NUGET_XMLDOC_MODE skip
RUN mkdir warmup \
    && cd warmup \
    && dotnet new \
    && cd .. \
    && rm -rf warmup \
    && rm -rf /tmp/NuGetScratch

RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN echo "deb [arch=amd64] https://apt-mo.trafficmanager.net/repos/azure-cli/ wheezy main" | tee /etc/apt/sources.list.d/azure-cli.list && \
    apt-key adv --keyserver apt-mo.trafficmanager.net --recv-keys 417A0893 && \
    apt-get update && \
    apt-get install --no-install-recommends -y apt-transport-https && \
    apt-get install --no-install-recommends -y \
        azure-cli \
        nodejs \
        libssl-dev \
        libffi-dev \
        python-dev \
        build-essential && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
    apt-get autoremove -y && apt-get clean

RUN npm i -g bower