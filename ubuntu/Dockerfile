FROM ubuntu:18.04

RUN set -x \
  && apt-get update && apt-get install -y wget \
  && wget -q https://github.com/CraneStation/wasi-sdk/releases/download/wasi-sdk-8/wasi-sdk_8.0_amd64.deb \
  && dpkg -i wasi-sdk_8.0_amd64.deb \
  && rm -f wasi-sdk_8.0_amd64.deb \
  && apt-get purge -y wget && apt-get autoremove -y \
  && rm -rf /var/lib/apt/lists/* \
  && echo 'PATH=/opt/wasi-sdk/bin:$PATH' >> /etc/profile

ENV LANG C.UTF-8

ENV PATH /opt/wasi-sdk/bin:$PATH
