ARG VARIANT="3.10"
FROM mcr.microsoft.com/vscode/devcontainers/python:${VARIANT}

RUN sudo apt update && sudo apt upgrade -y
RUN sudo apt install -y python3-pip

RUN python3 -m pip install --upgrade pip
RUN python3 -m pip install --upgrade setuptools
RUN python3 -m pip install --upgrade wheel

RUN sudo apt install git -y

RUN python3 -m pip install pylint black mypy isort flake8 pytest Sphinx