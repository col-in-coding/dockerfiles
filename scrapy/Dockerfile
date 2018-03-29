# Use an official Python runtime as a parent image
FROM python:3.7-rc-stretch

# Install Scrapy
RUN apt-get update
RUN pip install Scrapy

# Create /usr/src/app fold
RUN mkdir -p /usr/src/app/

ENTRYPOINT  /bin/bash

# Set the working directory to /usr/src/app
WORKDIR /usr/src/app/
