FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash gcc libc-dev nasm=~$VERSION
