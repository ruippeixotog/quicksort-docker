FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash lua$VERSION-dev

RUN ln -s /usr/bin/lua$VERSION /usr/bin/lua
