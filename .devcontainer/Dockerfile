FROM ubuntu:latest
# Install git-secrets
ENV VERSION=1.3.0
RUN apt update && apt install -y curl git vim && apt clean
RUN curl -sSL https://github.com/awslabs/git-secrets/archive/refs/tags/${VERSION}.tar.gz -o gitsecrets.tar.gz && \
    tar -xzf gitsecrets.tar.gz && \
    rm /gitsecrets.tar.gz && mv git-secrets-${VERSION}/git-secrets /bin/