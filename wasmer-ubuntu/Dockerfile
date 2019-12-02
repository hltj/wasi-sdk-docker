FROM hltj/wasi-sdk:7.0-ubuntu

RUN set -x \
  && apt-get update && apt-get install -y wget \
  && wget -q https://github.com/wasmerio/wasmer/releases/download/0.8.0/wasmer-linux-amd64.tar.gz \
  && mkdir /opt/wasmer && tar xf wasmer-linux-amd64.tar.gz -C /opt/wasmer \
  && rm -f wasmer-linux-amd64.tar.gz \
  && apt-get purge -y wget && apt-get autoremove -y \
  && rm -rf /var/lib/apt/lists/* \
  && echo 'PATH=/opt/wasmer/bin:$PATH' >> /etc/profile

ENV PATH /opt/wasmer/bin:$PATH
