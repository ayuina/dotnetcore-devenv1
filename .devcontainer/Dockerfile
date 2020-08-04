FROM mcr.microsoft.com/dotnet/sdk:5.0-focal

RUN apt-get update -yq \
    # Install Docker CLI
    && apt-get install -yq apt-transport-https ca-certificates curl gnupg-agent software-properties-common lsb-release unzip \
    && curl -fsSL https://download.docker.com/linux/ubuntu/gpg | apt-key add - \
    && add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" \
    && apt-get update \
    && apt-get install -yq docker-ce-cli

