FROM debian
ARG VERSION
RUN apt-get update && \
  apt-get install -y bash gcc-multilib libc6-dev-i386 nasm=$VERSION* && \
  rm -rf /var/lib/apt/lists/*
