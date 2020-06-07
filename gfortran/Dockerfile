FROM alpine
ARG VERSION
RUN apk update && \
  apk add --no-cache bash libc-dev gfortran=~$VERSION
