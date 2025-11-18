FROM mcr.microsoft.com/devcontainers/base:bullseye

#Install Grype
RUN curl -sSfL https://raw.githubusercontent.com/anchore/grype/main/install.sh | sh -s -- -b /usr/local/bin

#Install httpie and jq
RUN apt-get update && \
    apt-get install -y httpie jq && \
    rm -rf /var/lib/apt/lists/*
