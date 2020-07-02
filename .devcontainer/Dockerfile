FROM ubuntu:20.04

RUN apt-get update && apt-get install -y unzip

ADD https://github.com/haskell/haskell-language-server/files/4819805/vscode-hie-server-0.0.40.vsix.zip /vsix/

RUN unzip /vsix/vscode-hie-server-0.0.40.vsix.zip -d /vsix && \
    rm /vsix/vscode-hie-server-0.0.40.vsix.zip
