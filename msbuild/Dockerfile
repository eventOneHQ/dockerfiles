FROM microsoft/iis

#RUN cmd @powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" \
#    && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

RUN powershell -NoProfile -Command Set-ExecutionPolicy Unrestricted

RUN powershell -NoProfile -Command \
    Add-WindowsFeature NET-Framework-45-ASPNET; \
    Add-WindowsFeature Web-Net-Ext45; \
    Add-WindowsFeature Web-Asp-Net45; \
    Add-WindowsFeature  Web-ISAPI-Ext; \
    Add-WindowsFeature  Web-ISAPI-Filter

RUN powershell -NoProfile -Command \
    $env:chocolateyUseWindowsCompression = 'false'; \
    "iwr https://chocolatey.org/install.ps1 -UseBasicParsing | Invoke-Expression"


RUN powershell add-windowsfeature web-asp-net45

RUN cmd SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin" \
    && choco install microsoft-build-tools -y --allow-empty-checksums -version 14.0.23107.10 \
    && choco install dotnet4.6-targetpack --allow-empty-checksums -y \
    && choco install nuget.commandline --allow-empty-checksums -y \
    && nuget install MSBuild.Microsoft.VisualStudio.Web.targets -Version 14.0.0.3 \
    && nuget install WebConfigTransformRunner -Version 1.0.0.1