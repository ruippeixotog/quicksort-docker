FROM debian
RUN apt-get update && \
  apt-get install -y bash wget openjdk-11-jdk unzip && \
  rm -rf /var/lib/apt/lists/*

ARG VERSION
RUN wget http://downloads.typesafe.com/scala/$VERSION/scala-$VERSION.deb && \
  dpkg -i scala-$VERSION.deb && \
  rm scala-$VERSION.deb
