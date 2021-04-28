FROM telegraf:latest

USER root

RUN apt-get update \
 && apt-get install -y \
	vim-tiny \
	flip \
  ca-certificates \
  iputils-ping \
  libssl-dev \
  curl \
  ceph \
 && apt-get -y clean \
 && rm -rf /var/lib/apt/lists/*
