# This Dockerfile follows the Dockerhub python image recommendations,
#   updated to reside in a .devcontainer folder.
# See "How to use this image" in https://hub.docker.com/_/python.

# python 3.8 base image per NIST ESV Client README.md
FROM python:3.8

WORKDIR /usr/src/app

COPY .devcontainer/requirements.txt ./
RUN pip3 --disable-pip-version-check --no-cache-dir -r install requirements.txt

# Supposedly VS Code will make a shallow clone of the repo instide the container
# COPY . .

# To DO: the client may be run with various options; 
#   there may not be a single statement that is suitable here.
# CMD [ "python", "./client.py" ]