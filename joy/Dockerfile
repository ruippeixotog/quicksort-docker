FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash build-base

RUN mkdir /var/lib/joy && cd /var/lib/joy && \
  wget http://joy-lang.org/c-sources/joy.tar.gz && \
  tar zxvf joy.tar.gz && \
  make && \
  ln -s /var/lib/joy/joy /usr/local/bin && \
  rm joy.tar.gz
