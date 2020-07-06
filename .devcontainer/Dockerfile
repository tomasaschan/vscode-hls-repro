FROM docker.pkg.github.com/tomasaschan/vscode-devcontainers/haskell:0.1

USER root

RUN apt-get update && apt-get install -y unzip libncurses-dev libtinfo5

ARG HIE_VSIX_URL=https://github.com/haskell/haskell-language-server/files/4871220/vscode-hie-server-0.1.0.vsix.zip

RUN mkdir /vsix && \
    curl -sL ${HIE_VSIX_URL} -o /vsix/vscode-hie-server.vsix.zip && \
    unzip /vsix/vscode-hie-server.vsix.zip -d /vsix && \
    rm /vsix/vscode-hie-server.vsix.zip && \
    mv /vsix/vscode-hie-server-*.vsix /vsix/vscode-hie-server.vsix

USER dev
