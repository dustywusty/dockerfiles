FROM ubuntu:latest
MAINTAINER Dustin Clark <dusty@isperldead.net>

# ..

RUN apt-get update \
 && apt-get install -y software-properties-common \
 && add-apt-repository ppa:saltstack/salt \
 && apt-get update \
 && apt-get install -y salt-minion \
 && rm -rf /var/lib/apt/lists/*

# ..

 ENTRYPOINT ["salt-minion"]
 CMD ["--help"]
