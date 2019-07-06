FROM ubuntu:18.04
# ubuntu + python2-dev environment for building TensorFlow
ARG DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install -y apt-utils &&\
    apt install -y python-dev python-pip &&\
    apt install -y pkg-config zip zlib1g-dev unzip && : for Bazel &&\
    apt install -y git &&\
    pip install -U six numpy wheel setuptools mock future>=0.17.1 &&\
    pip install -U keras_applications==1.0.6 --no-deps &&\
    pip install -U keras_preprocessing==1.0.5 --no-deps

