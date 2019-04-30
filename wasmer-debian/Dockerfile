FROM hltj/wasi-sdk:4.0-debian

RUN set -x \
  && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl \
  && curl -sLO https://github.com/wasmerio/wasmer/releases/download/0.4.0/wasmer-linux-amd64.tar.gz \
  && mkdir /opt/wasmer && tar xf wasmer-linux-amd64.tar.gz -C /opt/wasmer \
  && rm -f wasmer-linux-amd64.tar.gz \
  && apt-get purge -y curl && apt-get autoremove -y \
  && rm -rf /var/lib/apt/lists/* \
  && echo 'PATH=/opt/wasmer/bin:$PATH' >> /etc/profile

ENV PATH /opt/wasmer/bin:$PATH
