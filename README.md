# Dotfiles for development

This project aims at creating dev environment using devcontainer and setting up lazy vim. 

## Pre-Requisite
Install devcontainer-cli. It requires `docker` and `docker compose` to be installed on the local machine.
```bash
npm install -g @devcontainers/cli
```

## Install

You need to have those dotfiles on your laptop, mount them in your devcontainer using the option `--mount` of `devcontainer up` and have your devcontainer configuration file executing the `install.sh` script contained in those dotfiles.

## How to develop

Use the devcontainer contained in the project. To build the image:
```bash
devcontainer build --workspace-folder .
```
To start docker containers:
```bash
devcontainer up --workspace-folder . \
```
And to connect to the container and develop:
```bash
devcontainer exec --workspace-folder . bash
```

