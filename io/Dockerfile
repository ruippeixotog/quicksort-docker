FROM debian
RUN apt-get update && \
  apt-get install -y bash wget unzip && \
  rm -rf /var/lib/apt/lists/*

ARG VERSION
RUN wget http://iobin.suspended-chord.info/linux/iobin-linux-x64-deb-$VERSION.zip && \
  unzip -d /io iobin-linux-x64-deb-current.zip && \
  dpkg -i /io/*.deb && \
  rm -r /io iobin-linux-x64-deb-current.zip
