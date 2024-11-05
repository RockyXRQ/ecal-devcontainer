FROM ubuntu:22.04

RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y software-properties-common wget build-essential

RUN apt install python3-launchpadlib -y
RUN rm -rf ~/.launchpadlib/api.launchpad.net/cache/

RUN wget https://bootstrap.pypa.io/get-pip.py
RUN python3 get-pip.py

RUN add-apt-repository -y ppa:ecal/ecal-latest
RUN apt-get update
RUN apt-get install -y ecal

RUN apt install -y python3-ecal5
RUN apt install -y protobuf-compiler
RUN pip install protobuf

RUN pip install opencv-python

RUN apt install -y git
RUN apt install -y v4l-utils