FROM debian
ARG VERSION
RUN apt-get update && \
  apt-get install -y bash fp-compiler=$VERSION* && \
  rm -rf /var/lib/apt/lists/*

# config verbosity of Pascal compiler
RUN sed -i 's/^-l$//' /etc/fpc.cfg
