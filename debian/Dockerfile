FROM debian:stretch

RUN set -x \
  && apt-get update && apt-get install -y --no-install-recommends ca-certificates curl \
  && curl -sLO https://github.com/CraneStation/wasi-sdk/releases/download/wasi-sdk-4/wasi-sdk_4.0_amd64.deb \
  && dpkg -i wasi-sdk_4.0_amd64.deb \
  && rm -f wasi-sdk_4.0_amd64.deb \
  && apt-get purge -y curl && apt-get autoremove -y \
  && rm -rf /var/lib/apt/lists/* \
  && echo 'PATH=/opt/wasi-sdk/bin:$PATH' >> /etc/profile

ENV LANG C.UTF-8

ENV PATH /opt/wasi-sdk/bin:$PATH
