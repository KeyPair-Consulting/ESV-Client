# This Dockerfile follows the Dockerhub python image recommendations,
#   updated to reside in a .devcontainer folder.
# See "How to use this image" in https://hub.docker.com/_/python.

# python 3.8 base image per NIST ESV Client README.md
FROM python:3.8

WORKDIR /usr/src/app

COPY .devcontainer/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

# To DO: the client may be run with various options; 
#   there may not be a single statement that is suitable here.
# CMD [ "python", "./client.py" ]