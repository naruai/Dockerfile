FROM ubuntu:18.04
# ubuntu + python3-dev environment for building TensorFlow
ARG DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install -y apt-utils &&\
    apt install -y python3-dev python3-pip &&\
    apt install -y pkg-config zip zlib1g-dev unzip && : for Bazel &&\
    apt install -y git &&\
    ln -s /usr/bin/python3 /usr/bin/python &&\
    ln -s /usr/bin/pip3 /usr/bin/pip &&\
    pip install -U six numpy wheel setuptools mock 'future>=0.17.1' &&\
    pip install -U keras_applications==1.0.6 --no-deps &&\
    pip install -U keras_preprocessing==1.0.5 --no-deps

