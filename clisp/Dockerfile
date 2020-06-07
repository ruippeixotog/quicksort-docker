FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash && \
  apk add --no-cache clisp=~$VERSION --repository=http://dl-cdn.alpinelinux.org/alpine/edge/testing
