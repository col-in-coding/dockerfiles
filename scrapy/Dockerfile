# Use an official Python runtime as a parent image
FROM alpine:3.7

RUN apk update
RUN apk add python-dev curl libxml2-dev libxslt-dev libffi-dev gcc musl-dev libgcc openssl-dev

# Install Scrapy
RUN curl https://bootstrap.pypa.io/get-pip.py | python
RUN pip install scrapy \
    && pip install --upgrade pip \
    && pip install scrapyd

# Create /usr/src/app fold
RUN mkdir -p /usr/src/app/
# Set the working directory to /usr/src/app
WORKDIR /usr/src/app/

EXPOSE 6800

ENTRYPOINT ["/usr/bin/scrapyd"]
