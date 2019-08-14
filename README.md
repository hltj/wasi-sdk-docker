# Docker images for WASI-SDK

Docker images for [WASI-enabled C/C++ toolchain](https://github.com/CraneStation/wasi-sdk)

Docker Hub repository: [hltj/wasi-sdk](https://hub.docker.com/r/hltj/wasi-sdk)

## Tags and `Dockerfile` links

Docker images with WASI-SDK only:
- [`latest`, `ubuntu`, `6.0`, `6.0-ubuntu` (ubuntu/Dockerfile)](https://github.com/hltj/wasi-sdk-docker/blob/master/ubuntu/Dockerfile)
- [`debian`, `6.0-debian` (debian/Dockerfile)](https://github.com/hltj/wasi-sdk-docker/blob/master/debian/Dockerfile)
- legacy: [`5.0`, `5.0-ubuntu`](https://github.com/hltj/wasi-sdk-docker/blob/ed8085587ff8b653237e7e8aeac27acd3fc12432/ubuntu/Dockerfile), [`4.0`, `4.0-ubuntu`](https://github.com/hltj/wasi-sdk-docker/blob/9bcc83268b22126d8a3dcb32ef5b0930284bcecb/ubuntu/Dockerfile)
- legacy: [`5.0-debian`](https://github.com/hltj/wasi-sdk-docker/blob/ed8085587ff8b653237e7e8aeac27acd3fc12432/debian/Dockerfile), [`4.0-debian`](https://github.com/hltj/wasi-sdk-docker/blob/9bcc83268b22126d8a3dcb32ef5b0930284bcecb/debian/Dockerfile)

Docker images with WASI-SDK and wasmer runtime:
- [`wasmer`, `wasmer-ubuntu`, `6.0-wasmer`, `6.0-wasmer-ubuntu` (wasmer-ubuntu/Dockerfile)](https://github.com/hltj/wasi-sdk-docker/blob/master/wasmer-ubuntu/Dockerfile)
- [`wasmer-debian`, `6.0-wasmer-debian` (wasmer-debian/Dockerfile)](https://github.com/hltj/wasi-sdk-docker/blob/master/wasmer-debian/Dockerfile)
- legacy: [`5.0-wasmer`, `5.0-wasmer-ubuntu`](https://github.com/hltj/wasi-sdk-docker/blob/ed8085587ff8b653237e7e8aeac27acd3fc12432/wasmer-ubuntu/Dockerfile), [`4.0-wasmer`, `4.0-wasmer-ubuntu`](https://github.com/hltj/wasi-sdk-docker/blob/9bcc83268b22126d8a3dcb32ef5b0930284bcecb/wasmer-ubuntu/Dockerfile)
- legacy: [`5.0-wasmer-debian`](https://github.com/hltj/wasi-sdk-docker/blob/ed8085587ff8b653237e7e8aeac27acd3fc12432/wasmer-debian/Dockerfile), [`4.0-wasmer-debian`](https://github.com/hltj/wasi-sdk-docker/blob/9bcc83268b22126d8a3dcb32ef5b0930284bcecb/wasmer-debian/Dockerfile)
