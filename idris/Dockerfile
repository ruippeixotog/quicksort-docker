FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash libc-dev && \
  apk add --no-cache idris=~$VERSION --repository=http://dl-cdn.alpinelinux.org/alpine/edge/testing
