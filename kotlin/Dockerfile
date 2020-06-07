FROM debian
RUN apt-get update && \
  apt-get install -y bash wget openjdk-11-jdk unzip && \
  rm -rf /var/lib/apt/lists/*

ARG VERSION
RUN wget https://github.com/JetBrains/kotlin/releases/download/v$VERSION/kotlin-compiler-$VERSION.zip && \
  unzip -d /opt kotlin-compiler-$VERSION.zip && \
  ln -s /opt/kotlinc/bin/kotlinc /usr/local/bin && \
  ln -s /opt/kotlinc/bin/kotlin /usr/local/bin && \
  rm kotlin-compiler-$VERSION.zip
